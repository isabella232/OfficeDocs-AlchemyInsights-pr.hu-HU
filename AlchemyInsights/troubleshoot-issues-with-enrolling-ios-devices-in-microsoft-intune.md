---
title: IOS-eszközök regisztrálásával kapcsolatos hibák elhárítása a Microsoft Intune
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
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047978"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>IOS-eszközök regisztrálásával kapcsolatos hibák elhárítása a Microsoft Intune

A probléma megoldásához tekintse át az alábbi forrásokat. 
  
Gyakori hibaüzenetek és megoldási lépések:
  
- **Eszköz cap reached** A felhasználónak több eszköze van regisztrálva, mint az eszközkorlát. Ezeket a dokumentumokat áttekintve [eltávolíthat egy eszközt,](https://docs.microsoft.com/intune/devices-wipe) [vagy módosíthatja az eszközkorlátot.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Ez a szolgáltatás nem támogatott. Nincs regisztrációs házirend:** Az Apple leküldéses értesítéseket szolgáltató szolgáltatását konfigurálni vagy meg kell újítani. Ennek [utasításokért](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) tekintse át ezt a dokumentumot. 
    
- **Érvénytelen felhasználói licenctípus, vagy nem ismerhető fel a felhasználónév:** A felhasználónak Intune- vagy EMS-licencet kell hozzárendelni. A licencek hozzárendeléshez tekintse át az alábbi dokumentumokat: Office [Felügyeleti központ vagy](https://docs.microsoft.com/intune/licenses-assign) Azure [Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups)webhelyen.
    
További források a probléma megoldásához:
  
1. Az [Intune hibaelhárítási portálján diagnosztizálhatja](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) és megoldhatja a gyakori regisztrációs hibákat. További [részleteket ebben](https://docs.microsoft.com/intune/help-desk-operators) a dokumentumban talál. 
    
2. Az alábbi dokumentumokban áttekintheti azoknak a gyakori hibáknak a listáját, amelyek meggátolják az regisztrációt és megoldást: [Hibaelhárítási útmutató](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és a [Hibaelhárítási dokumentum](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Megtudhatja, hogy miként regisztrálja az iOS-eszközöket a Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

