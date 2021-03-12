---
title: Az iOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708964"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Az iOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos hibák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat. 
  
Néhány gyakori hibaüzenet és megoldási lépés:
  
- **Eszköz cap reached** A felhasználó több eszközt regisztrált, mint az eszközkorlát. Ezeket a dokumentumokat áttekintve [eltávolíthat egy eszközt,](https://docs.microsoft.com/intune/devices-wipe) vagy [módosíthatja az eszközkorlátot.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Ez a szolgáltatás nem támogatott. Nincs regisztrációs házirend:** Az Apple leküldéses értesítési szolgáltatását (APNS) konfigurálni vagy meg kell újítani. Ennek [mikéntjére](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) vonatkozó utasításokat ebben a dokumentumban tud meg. 
    
- **A felhasználói licenc típusa érvénytelen vagy a felhasználónév nem ismerhető fel:** A felhasználónak Intune- vagy EMS-licencet kell hozzárendelni. Tekintse át az alábbi dokumentumokat, és rendeljen licencet a következőn keresztül: [Office Felügyeleti központ](https://docs.microsoft.com/intune/licenses-assign) vagy Azure [Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
További források a probléma megoldásához:
  
1. Az [Intune hibaelhárítási portálján](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és megoldhatja a gyakori regisztrációs hibákat. További [részletekért tekintse](https://docs.microsoft.com/intune/help-desk-operators) át ezt a dokumentumot. 
    
2. Az alábbi dokumentumokban áttekintheti azokat a gyakori hibákat, [](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) amelyek meggátolják a regisztrációt és az egyes problémák megoldását: hibaelhárítási útmutató és [hibaelhárítási dokumentum.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Megtudhatja, hogy miként regisztrálható iOS-eszközök a Microsoft Intune-ban.](https://docs.microsoft.com/intune/ios-enroll)
    

