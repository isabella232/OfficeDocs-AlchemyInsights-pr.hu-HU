---
title: Eszköz függőben lévő állapotban
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330374"
---
# <a name="device-in-pending-state"></a>Eszköz függőben lévő állapotban

**Előfeltételek:**

1. Ha első alkalommal ad meg eszközregisztrációkat, kérjük, tekintse át a Bevezetés az eszközkezelésbe az [Azure Active Directory -ban (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) bemutatót, amely útmutatást ad arról, hogy miként irányíthatja az eszközöket az Azure AD irányításához.
2. Ha közvetlenül regisztrál eszközöket az Azure AD-be, és regisztrálja őket az Intune-ba, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) először meg kell bizonyosodnia arról, hogy konfigurálta az [Intune-t,](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) és megfelelően beállította a licencelést.
3. Győződjön meg arról, hogy jogosult műveletek elvégzésére az Azure AD-ban és a helyszíni AD-ban. Az eszközregisztrációk beállításait csak az Azure AD globális rendszergazdája kezelheti. Ezenkívül ha automatikus regisztrációt hoz létre a helyszíni Active Directoryban, akkor az Active Directory és az Active Directory FS (ha van) rendszergazdájának kell lennie.

A hibrid Azure AD-csatlakozás regisztrációs folyamata megköveteli, hogy az eszközök vállalati hálózatot használjanak. A VPN-en keresztül is működik, de ennek vannak kikötései. Ügyfeleink szerint távoli munkahelyi körülmények között segítségre van szükségük az Azure AD bekapcsolódási folyamatának hibaelhárításához.

**Felhőalapú hitelesítési környezet (Azure AD-jelszó kivonatszinkronizálás vagy átmenő hitelesítés használata)**

Ezt a regisztrációs folyamatot szinkronizálási illesztésnek is nevezik.

Az alábbi részletezés be van lebontva arra, hogy mi történik a regisztrációs folyamat során:

1. Windows 10 szolgáltatás csatlakozási pont (SCP) rekordját, amikor a felhasználó bejelentkezik az eszközre.

    1. Az eszköz először megpróbálja lekérni a bérlői adatokat az ügyféloldali SCP-értékből a beállításjegyzékben [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. További információ: [dokumentum.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Ha nem sikerül, az eszköz a helyszíni Active Directoryval kommunikálva bekérte a bérlői adatokat az SCP-től. Az SCP ellenőrzéséhez tanulmányozza ezt a [dokumentumot.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    **Megjegyzés: Azt** javasoljuk, hogy az Active Directoryban engedélyezi az SCP-t, és csak az ügyféloldali SCP-t használja a kezdeti ellenőrzéshez.

2. Windows 10 megpróbál kommunikálni az Azure AD-val a rendszerkörnyezetben, hogy hitelesítse magát az Azure AD-val.

    Ha ellenőrizni tudja, hogy az eszköz hozzáfér-e a Microsoft-erőforrásokhoz a rendszerfiók alatt, használja az Eszköz-regisztrációs kapcsolat tesztelése [parancsprogramot.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 önaírt tanúsítványt hoz létre, és a számítógép-objektum alatt tárolja a helyszíni Active Directoryban. Ehhez szem előtt kell lennie a tartományvezérlőnek.

4. A tanúsítvánnyal rendelkezik eszközobjektumot a rendszer szinkronizálja az Azure AD szolgáltatáson keresztül az Azure AD Csatlakozás. A szinkronizálási ciklus alapértelmezés szerint 30 percenként van, de attól függ, hogy az Azure AD hogyan Csatlakozás. További információért olvassa el ezt a [dokumentumot.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Ebben a fázisban az Azure Portal eszközszála alatt látható a tárgyeszköz " függőben **"** állapota.

6. A bejelentkezéshez a következő Windows 10 a regisztrációt.

    **Megjegyzés:** Ha VPN-t használ, és az embléma/bejelentkezés megszünteti a tartomány csatlakozását, manuálisan elindíthatja a regisztrációt. A következőt kell tenni:
    
    Helyi probléma `dsregcmd /join` megoldása rendszergazdai üzenetben vagy a PSExecen keresztül a PC-n keresztül.\
    Például: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Az eszközregisztrációval kapcsolatos gyakori Azure Active Directory olvassa el az Eszközök – gyakori [kérdések című témakört.](https://docs.microsoft.com/azure/active-directory/devices/faq)
