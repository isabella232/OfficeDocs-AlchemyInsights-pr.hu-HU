---
title: Az iOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823465"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Az iOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat. 
  
Gyakori hibaüzenetek és megoldási lépések:
  
- **Eszköz cap reached** A felhasználónak több eszköze van regisztrálva, mint az eszközkorlát. Ezeket a dokumentumokat áttekintve [eltávolíthat egy eszközt,](https://docs.microsoft.com/intune/devices-wipe) [vagy módosíthatja az eszközkorlátot.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Ez a szolgáltatás nem támogatott. Nincs regisztrációs házirend:** Az Apple leküldéses értesítéseket szolgáltató szolgáltatását konfigurálni vagy meg kell újítani. Ennek [utasításokért](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) tekintse át ezt a dokumentumot. 
    
- **Érvénytelen felhasználói licenctípus, vagy nem ismerhető fel a felhasználónév:** A felhasználónak Intune- vagy EMS-licencet kell hozzárendelni. A következő dokumentumok alapján rendeljen licencet: [Office Felügyeleti központ](https://docs.microsoft.com/intune/licenses-assign) vagy Azure [Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
További források a probléma megoldásához:
  
1. Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat. További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál. 
    
2. Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, amelyek meggátolják az egyes dokumentumok regisztrálását és megoldását: [Hibaelhárítási](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) útmutató és Hibaelhárítási [dokumentum.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Megtudhatja, hogy miként regisztrálható az iOS-eszközök a Microsoft Intune-ban.](https://docs.microsoft.com/intune/ios-enroll)
    

