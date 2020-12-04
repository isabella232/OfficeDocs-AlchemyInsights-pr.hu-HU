---
title: PRT-s probléma elhárítása
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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573717"
---
# <a name="troubleshoot-prt-issue"></a>PRT-s probléma elhárítása

Ahhoz, hogy bármilyen eszköz hitelesítve legyen, teljes mértékben be kell jegyeztetni, és jó állapotban kell lennie, és az elsődleges frissítési tokent (PRT) meg kell szereznie.

A hibrid Azure AD csatlakozás regisztrációs folyamathoz az eszközöknek vállalati hálózaton kell lenniük. Ez a funkció többek között a VPN-en is működik, de van némi kikötése. Hallottuk, hogy az ügyfelek segítségre szorulnak a hibrid Azure AD-csatlakozás regisztrációjának hibaelhárításához a távoli munka körülményei között. Az alábbiakban felsoroljuk, hogy mi történik a regisztrációs folyamat során a motorháztető alatt.

**Felhőalapú hitelesítési környezet (az Azure AD Password hash szinkronizálása vagy a továbbítás hitelesítése)**

Ez a regisztrációs folyamat "szinkronizálási csatlakozás" néven is ismert.

1. A Windows 10 a felhasználó által az eszközre való bejelentkezéskor megtalál egy SCP-rekordot.
    1. Az eszköz először az ügyféloldali SCP-ből kísérli meg beolvasni a bérlői adatokat a beállításjegyzékben [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. További információt ebben a [dokumentumban](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)talál.
    2. Ha nem működik, az eszköz a helyszíni Active Directoryval (AD) kommunikál a bérlői adatok eléréséhez a Service Connection Pointból (SCP). A SZOLGÁLTATÁSKAPCSOLÓDÁSI pont ellenőrzéséhez olvassa el ezt a [dokumentumot](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Javasoljuk, hogy engedélyezze az SCP használatát a HIRDETÉSben, és csak az ügyféloldali szolgáltatáskapcsolódási pontok használatát a kezdeti ellenőrzéshez.

2. A Windows 10 a rendszerkörnyezetben próbál meg kommunikálni az Azure AD szolgáltatással, és az Azure AD-ot használva hitelesíti magát. Ellenőrizheti, hogy az eszköz hozzáférhet-e a Microsoft-erőforrásokhoz a rendszerfiók csoportban a számítógép-nyilvántartási csatlakozási parancsfájl használatával.

3. A Windows 10 létrehoz egy önaláírt tanúsítványt, és a számítógép-objektum alatt tárolja a helyszíni hirdetések között. Ehhez a tartományvezérlőt kell megadnia.

4. A tanúsítványt tartalmazó eszköz-objektum az Azure ad Connect segítségével szinkronizálódik az Azure AD-kapcsolaton keresztül. A szinkronizálási ciklus alapértelmezés szerint 30 percenként van, de az Azure AD Connect konfigurációjától függ. További információért olvassa el ezt a [dokumentumot](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Ebben a szakaszban látnia kell a tárgy eszközt "függőben" állapotban az Azure-portál eszköz Blade területén.

6. A Windows 10 rendszer következő felhasználó bejelentkezésekor a regisztráció be lesz töltve. 

> [!NOTE]
> Ha a VPN-en tartózkodik, és a kijelentkezési bejelentkezési folyamat lemondja a tartomány kapcsolatát, a regisztrációt kézzel is aktiválhatja:
 1. Dsregcmd/JOIN a rendszergazdától, vagy távolról a PSExec-on keresztül a számítógépre. Például PsExec-s \\ win10client01 cmd, dsregcmd/JOIN

 2. A hibrid kapcsolódási problémákkal kapcsolatos további részletekért olvassa el az [eszközökkel kapcsolatos problémák elhárítása](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)című témakört.
