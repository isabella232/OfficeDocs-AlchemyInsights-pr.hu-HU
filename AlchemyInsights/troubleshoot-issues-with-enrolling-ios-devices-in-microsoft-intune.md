---
title: IOS-eszközökkel kapcsolatos problémák elhárítása a Microsoft Intune-ben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507005"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>IOS-eszközökkel kapcsolatos problémák elhárítása a Microsoft Intune-ben

A probléma megoldásához tekintse át az alább felsorolt erőforrásokat. 
  
Gyakori hibaüzenetek és megoldási lépések:
  
- A **Device Cap elérte** A felhasználó több, az eszközkorlátnál igényléssel rendelkező eszközzel rendelkezik. Ellenőrizze ezeket a dokumentumokat az [eszköz eltávolításához](https://docs.microsoft.com/intune/devices-wipe) vagy [az eszközkorlát megváltoztatásához](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ez a szolgáltatás nem támogatott. Nem besorozás politika:** Alma támadás hirdetés szolgáltatás (APNS) szükséges-hoz lenni configured vagy megújít. Olvassa el [ezt a dokumentumot](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , hogy hogyan kell ezt megtenni. 
    
- **Érvénytelen felhasználói licenctípus, vagy a felhasználó neve nem ismerhető fel:** A felhasználónak Intune-vagy EMS-licencet kell rendelni. Tekintse át ezeket a dokumentumokat, és rendeljen hozzá licencet az [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) vagy az [Azure Portal webhelyen](https://docs.microsoft.com/azure/active-directory/license-users-groups)keresztül.
    
További források a probléma megoldásához:
  
1. Az [Intune – hibaelhárítás portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) használatával diagnosztizálhatja és megoldhatja a gyakori igénylési hibákat. További részletekért olvassa el [ezt a dokumentumot](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Tekintse át ezeket a dokumentumokat az olyan gyakori hibák listájához, amelyek megakadályozzák a tanúsítványigénylést és az egyes felbontásokat: [hibaelhárítási útmutató](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és a [doc-hibaelhárítás](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Információ az iOS-eszközök Microsoft Intune szolgáltatással történő igényléséről](https://docs.microsoft.com/intune/ios-enroll).
    

