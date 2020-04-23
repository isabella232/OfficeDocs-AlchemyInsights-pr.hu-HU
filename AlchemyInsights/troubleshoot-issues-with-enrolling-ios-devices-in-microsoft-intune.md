---
title: IOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736160"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>IOS-eszközök Microsoft Intune-ban való regisztrálásával kapcsolatos problémák elhárítása

A probléma megoldásához tekintse át az alábbi forrásokat. 
  
Néhány gyakori hibaüzenet és megoldási lépés:
  
- **Elérte az eszközkorlátot** A felhasználó több eszközt regisztrált, mint az eszköz korlátját. Tekintse át ezeket a dokumentumokat [az eszköz eltávolításához](https://docs.microsoft.com/intune/devices-wipe) vagy [az eszközkorlát módosításához.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Ez a szolgáltatás nem támogatott. Nincs regisztrációs szabályzat:** Az Apple leküldéses értesítési szolgáltatását (APNS) konfigurálni vagy megújítani kell. Tekintse át ezt a [dokumentumot,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) hogy ennek hogyan tehető. 
    
- **Érvénytelen felhasználói licenctípus vagy nem felismert felhasználónév:** A felhasználónak Intune- vagy EMS-licencet kell hozzárendelnie. Tekintse át ezeket a dokumentumokat, hogy licencet rendeljen az [Office Felügyeleti központon](https://docs.microsoft.com/intune/licenses-assign) vagy [az Azure Portalon](https://docs.microsoft.com/azure/active-directory/license-users-groups)keresztül.
    
További források a probléma megoldásához:
  
1. Az [Intune hibaelhárítási portáljával](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosztizálhatja és feloldhatja a gyakori regisztrációs hibákat. Tekintse át ezt a [dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) további részletekért. 
    
2. Tekintse át ezeket a dokumentumokat a gyakori hibák listájáért, amelyek megakadályozzák a regisztrációt és az egyes megoldásokat: [Hibaelhárítási útmutató](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és [hibaelhárítás idopont](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Megtudhatja, hogy miként regisztrálhatja az iOS-eszközöket a Microsoft Intune-ban.](https://docs.microsoft.com/intune/ios-enroll)
    

