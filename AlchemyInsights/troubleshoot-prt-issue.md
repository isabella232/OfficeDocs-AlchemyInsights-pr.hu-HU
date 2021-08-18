---
title: PRT-probléma elhárítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330961"
---
# <a name="troubleshoot-prt-issue"></a>PRT-probléma elhárítása

A hitelesítés befejezéséhez minden eszköznek teljes regisztrálva kell lennie, és jó állapotban kell lennie, és hozzá kell szereznie egy elsődleges frissítési jogkivonatot (PRT).

A hibrid Azure AD-csatlakozás regisztrációs folyamata megköveteli, hogy az eszközök vállalati hálózaton csatlakozzanak. A VPN-en keresztül is működik, de ennek vannak kikötései. Azt halljuk, hogy ügyfeleinknek segítségre van szükségük a hibrid Azure AD-bekapcsolódási regisztrációs folyamat hibaelhárításához távoli munkahelyi körülmények között. Az alábbi részletezésben arról lesz szó, hogy mi történik "a motorháztető alatt" a regisztrációs folyamat során.

**Felhőalapú hitelesítési környezet (Azure AD-jelszó kivonatszinkronizálás vagy átmenő hitelesítés használata)**

Ezt a regisztrációs folyamatot szinkronizálási illesztésnek is nevezik.

1. Windows 10 SCP-rekordot fedez fel, amikor a felhasználó bejelentkezik az eszközre.
    1. Az eszköz először megpróbálja lekérni a bérlői adatokat az ügyféloldali SCP-értékből a beállításjegyzékben [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. További információ ebben a [dokumentumban található.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Ha nem sikerül, az eszköz a helyszíni Active Directoryval (AD) kommunikálva beszerszi a bérlő adatait a Service Connection Point (SCP) szolgáltatásból. Az SCP ellenőrzéséhez tanulmányozza ezt a [dokumentumot.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

**Megjegyzés:** Azt javasoljuk, hogy az AD-ben engedélyezi az SCP-t, és csak az ügyféloldali SCP-et használja a kezdeti ellenőrzéshez.

2. Windows 10 megpróbál kommunikálni az Azure AD-val a rendszerkörnyezetben, hogy hitelesítse magát az Azure AD-val. Az Eszköz-regisztrációs kapcsolat tesztelése parancsprogramot használva ellenőrizheti, hogy az eszköz hozzáfér-e a rendszerfiók microsoftos erőforrásaihoz.

3. Windows 10 önaírt tanúsítványt hoz létre, és a számítógép-objektum alatt tárolja a helyszíni AD-ban. Ehhez szem előtt kell lennie a tartományvezérlőnek.

4. A tanúsítvánnyal rendelkezik eszközobjektumokat a rendszer szinkronizálja az Azure AD szolgáltatáson keresztül az Azure AD Csatlakozás. A szinkronizálási ciklus alapértelmezés szerint 30 percenként van, de az Azure AD-szolgáltatások beállításaitól Csatlakozás. További információért olvassa el ezt a [dokumentumot.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Ebben a fázisban a tárgyeszközt "Függőben" állapotban kell látnia az Azure Portal Eszközszála alatt.

6. A bejelentkezéshez a következő Windows 10 a regisztrációt. 

**Megjegyzés:** Ha VPN-t használ, és egy embléma-bejelentkezési folyamat megszünteti a tartomány csatlakozását, manuálisan elindíthatja a regisztrációt:
 1. Dsregcmd /join hibát ad meg helyileg egy rendszergazdai üzenetben, vagy távolról, a PSExecen keresztül a PC-n. Például: PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. A Hibrid csatlakozással kapcsolatos problémákról az Eszközproblémák elhárítása [témakörben olvashat bővebben.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
