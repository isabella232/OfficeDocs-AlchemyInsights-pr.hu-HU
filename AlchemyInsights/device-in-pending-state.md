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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914005"
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

    > [!NOTE]
    > Azt javasoljuk, hogy az Active Directoryban engedélyezi az SCP-t, és csak ügyféloldali SCP-t használva.

2. Windows 10 megpróbál kommunikálni az Azure AD-val a rendszerkörnyezetben, hogy hitelesítse magát az Azure AD-val.

    Az Eszköz-regisztrációs kapcsolat tesztelése parancsprogramot használva ellenőrizheti, hogy az eszköz hozzáfér-e a rendszerfiók microsoftos [erőforrásaihoz.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 önaírt tanúsítványt hoz létre, és a számítógép-objektum alatt tárolja a helyszíni Active Directoryban. Ehhez szem előtt kell lennie a tartományvezérlőnek.

4. A tanúsítvánnyal rendelkezik eszközobjektumot a rendszer szinkronizálja az Azure AD szolgáltatáson keresztül az Azure AD Csatlakozás. A szinkronizálási ciklus alapértelmezés szerint 30 percenként van, de attól függ, hogy hogyan van konfigurálva az Azure AD Csatlakozás. További információért olvassa el ezt a [dokumentumot.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Ebben a fázisban az Azure Portal eszközszála alatt látható a tárgyeszköz " függőben **"** állapota.

6. A bejelentkezéshez a következő Windows 10 a regisztrációt.

    > [!NOTE]
    > Ha VPN-t használ, és az embléma/bejelentkezés megszünteti a tartomány csatlakozását, manuálisan elindíthatja a regisztrációt. A következőt kell tenni:
    >
    > Helyileg vagy a PSExecen keresztül a PC-n keresztül helyileg is közzétehető `dsregcmd /join` rendszergazdai kérést ad.
    >
    > Például: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Az eszközregisztrációval kapcsolatos gyakori Azure Active Directory olvassa el az Eszközök – gyakori [kérdések című témakört.](https://docs.microsoft.com/azure/active-directory/devices/faq)
