---
title: Igénylése a Microsoft Intune iOS-eszközök problémáinak elhárítása
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507005"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Igénylése a Microsoft Intune iOS-eszközök problémáinak elhárítása

Most a probléma megoldásához kövesse az alább felsorolt erőforrások áttekintése. 
  
Néhány gyakori hibaüzenetek és a megoldás lépéseit:
  
- **Elérhető eszközt kap** A felhasználó rendelkezik az eszköz által megszabott mint igényelt további eszközöket. Tekintse át [az eszköz eltávolítása](https://docs.microsoft.com/intune/devices-wipe) vagy [módosítása az eszköz által megszabott](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)e dokumentumokat.
    
- A szolgáltatás **nem támogatott. Nincs tanúsítványigénylési házirend:** Apple leküldéses értesítési szolgáltatás (hozzáférésipont-nevek tartoznak) kell konfigurálni vagy megújítani. [Ez a dokumentum](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) útmutatást ehhez áttekintése. 
    
- **Felhasználói licenc érvénytelen vagy ismeretlen felhasználónév:** A felhasználónak kell egy Intune vagy EMS licencet kap. Tekintse át ezeket a dokumentumokat keresztül licenc hozzárendelése: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) vagy [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
A probléma megoldásához további erőforrások:
  
1. [Intune hibaelhárítás Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) segítségével azonosíthatja és megoldhatja a beiktatási gyakori hibák. [Ez a dokumentum](https://docs.microsoft.com/intune/help-desk-operators) további részletekért tekintse át. 
    
2. Tekintse át ezeket a dokumentumokat, amelyek megakadályozzák a tanúsítványigénylési és -megoldások egyes gyakori hibák listája: [Útmutató a hibaelhárítás](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) és a [Hibaelhárítás doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Útmutató a Microsoft Intune iOS-eszközök igénylésére](https://docs.microsoft.com/intune/ios-enroll).
    

