---
title: A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808973"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>A Windows-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat.
  
Gyakori hibaüzenetek és megoldási lépések:
  
 **A szoftvert nem lehet telepíteni, mert ez 0x80cf4017:** A fiók tanúsítványa lejárt. Töltse le újra a PC-ügyfélszoftver csomagját az Intune Felügyeleti konzolon. További információt ebben a dokumentációban talál.
  
 **Hibakód 0x801c0003:** A hiba az alábbi esetekben fordulhat elő:
  
-  A felhasználónak több eszköze van regisztrálva, mint az eszközkorlát. Ezeket a dokumentumokat áttekintve [eltávolíthat egy eszközt,](https://docs.microsoft.com/intune/devices-wipe) [vagy módosíthatja az eszközkorlátot.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  A "Felhasználók csatlakozhatnak az Azure AD-hez" beállítás "nincs" beállításra van állítva. Állítsa be az összes felhasználóra, vagy válassza ki a kívánt felhasználókat. További [információt ebben](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) a dokumentációban talál.

-  Az eszközt már regisztrálta egy másik felhasználó. Ha ez a helyzet, távolítsa el az eszközt az Azure Intune konzolból, vagy manuálisan törölje az eszköz igénylését, mielőtt újra próbálkozik.

-  Az eszköz a Windows 10 Home. Csak a Windows 10 Pro, az Oktatási és a Nagyvállalati verziós előfizetések csatlakozhatnak az Azure Active Directoryhoz.

További források a probléma megoldásához:
  
-  Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat. További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál.

-  Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, amelyek meggátolják az egyes dokumentumok regisztrálását és megoldását: [Hibaelhárítási](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) útmutató és Hibaelhárítási [dokumentum.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Megtudhatja, hogy miként regisztrálja a Windows-eszközöket a Microsoft Intune-ban.](https://docs.microsoft.com/intune/windows-enroll)
