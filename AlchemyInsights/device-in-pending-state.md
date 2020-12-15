---
title: Eszköz függőben állapotban
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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678482"
---
# <a name="device-in-pending-state"></a>Eszköz függőben állapotban

**Előfeltételek**

1. Ha első alkalommal állítja be az eszközök regisztrációját, győződjön meg arról, hogy az Azure Active Directory-ban az Azure Active Directory-ban áttekintheti az [eszközillesztők bevezetését](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , amely bemutatja, hogy miként szerezhet be eszközöket az Azure ad felügyelete alá.
2. Ha közvetlenül az Azure AD-ba jelentkezik be, és beiratkozik őket a Intune-ba, gondoskodnia kell arról, hogy az Intune-t [konfigurálta](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) , és először a [licencet](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) állítsa be.
3. Ellenőrizze, hogy jogosult-e műveletek végrehajtására az Azure AD-ban és a helyszíni AD-ban. Az Azure AD szolgáltatásban csak egy globális rendszergazda kezelhetik az eszközök regisztrációjának beállításait. Ha a helyszíni Active Directoryban automatikus regisztrációkat állít be, az Active Directory és az Active Directory összevonási szolgáltatások (ha szükséges) rendszergazdájának kell lennie.

A hibrid Azure AD csatlakozás regisztrációs folyamathoz a vállalati hálózatban lévő eszközökre van szükség. Ez a funkció többek között a VPN-en is működik, de van némi kikötése. Hallottuk, hogy az ügyfelek segítségre szorulnak a hibrid Azure AD-csatlakozás regisztrációs folyamatának hibaelhárítása távoli munkakörülmények között.

**Felhőalapú hitelesítési környezet (az Azure AD Password hash szinkronizálása vagy a továbbítás hitelesítése)**

Ez a regisztrációs folyamat "szinkronizálási csatlakozás" néven is ismert.

Itt megtudhatja, hogy mi történik a regisztrációs folyamat során:

1. A Windows 10 feltárta a Service Connection Point (SCP) rekordját, amikor a felhasználó bejelentkezik az eszközre.

    1. Az eszköz először az ügyféloldali SCP-ből kísérli meg beolvasni a bérlői adatokat a beállításjegyzékben [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. További információt a [dokumentum](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)című témakörben találhat.
    1. Ha nem működik, az eszköz a helyszíni Active Directoryval kommunikál a bérlői adatoknak a SZOLGÁLTATÁSKAPCSOLÓDÁSI pontból való beszerzéséhez. A SZOLGÁLTATÁSKAPCSOLÓDÁSI pont ellenőrzéséhez tekintse át ezt a [dokumentumot](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Javasoljuk, hogy engedélyezze az SCP használatát az Active Directoryban, és csak ügyféloldali szolgáltatáskapcsolódási pontok használatát a kezdeti ellenőrzéshez.

2. A Windows 10 a rendszerkörnyezetben próbál meg kommunikálni az Azure AD szolgáltatással, és az Azure AD-ot használva hitelesíti magát.

    Ellenőrizheti, hogy az eszköz hozzáférhet-e a Microsoft-erőforrásokhoz a rendszerfiók csoportban a számítógép- [nyilvántartási csatlakozási parancsfájl](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)használatával.

3. A Windows 10 önaláírt tanúsítványt hoz létre, és a számítógép-objektum alatt tárolja a helyszíni Active Directoryban. Ehhez a tartományvezérlőt kell megadnia.

4. A tanúsítványt tartalmazó eszköz-objektum az Azure ad Connecten keresztül szinkronizálódik az Azure AD-hoz. A szinkronizálási ciklus alapértelmezés szerint minden 30 perc, de az Azure AD Connect konfigurációjától függ. További információért olvassa el ezt a [dokumentumot](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Ebben a szakaszban látnia kell a tárgy eszközt "**függőben**" állapotban az Azure-portál eszköz Blade területén.

6. A Windows 10 rendszer következő felhasználó bejelentkezésekor a regisztráció be lesz töltve.

    > [!NOTE]
    > Ha a VPN és a kijelentkezés/bejelentkezés funkció lemondja a tartomány kapcsolatát, akkor a regisztrációt kézzel is aktiválhatja. Teendő:
    >
    > Az `dsregcmd /join` PSExec-on keresztül távolról, a számítógépén keresztül is kiadhatja a helyileg a rendszergazdát.
    >
    > Példa: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Az Azure Active Directory-regisztrációval kapcsolatos gyakori problémák az [eszközök – gyakori kérdések](https://docs.microsoft.com/azure/active-directory/devices/faq)című témakörben olvashatók.
