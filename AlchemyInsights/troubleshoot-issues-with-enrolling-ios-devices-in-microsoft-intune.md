---
title: Igénylése a Microsoft Intune iOS-eszközök problémáinak elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28294246"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Igénylése a Microsoft Intune iOS-eszközök problémáinak elhárítása

Most a probléma megoldásához kövesse az alább felsorolt erőforrások áttekintése. 
  
Néhány gyakori hibaüzenetek és a megoldás lépéseit:
  
- **Elérhető eszközt kap** A felhasználó rendelkezik az eszköz által megszabott mint igényelt további eszközöket. Tekintse át [az eszköz eltávolítása](https://docs.microsoft.com/en-us/intune/devices-wipe) vagy [módosítása az eszköz által megszabott](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)e dokumentumokat.
    
- A szolgáltatás **nem támogatott. Nincs tanúsítványigénylési házirend:** Apple leküldéses értesítési szolgáltatás (hozzáférésipont-nevek tartoznak) kell konfigurálni vagy megújítani. [Ez a dokumentum](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) útmutatást ehhez áttekintése. 
    
- **Felhasználói licenc érvénytelen vagy ismeretlen felhasználónév:** A felhasználónak kell egy Intune vagy EMS licencet kap. Tekintse át ezeket a dokumentumokat keresztül licenc hozzárendelése: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) vagy [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).
    
A probléma megoldásához további erőforrások:
  
1. [Intune hibaelhárítás Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) segítségével azonosíthatja és megoldhatja a beiktatási gyakori hibák. [Ez a dokumentum](https://docs.microsoft.com/en-us/intune/help-desk-operators) további részletekért tekintse át. 
    
2. Tekintse át ezeket a dokumentumokat, amelyek megakadályozzák a tanúsítványigénylési és -megoldások egyes gyakori hibák listája: [Útmutató a hibaelhárítás](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és a [Hibaelhárítás doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Útmutató a Microsoft Intune iOS-eszközök igénylésére](https://docs.microsoft.com/en-us/intune/ios-enroll).
    

