---
title: Igénylése a Windows Microsoft Intune-eszközök problémáinak elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934778"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Igénylése a Windows Microsoft Intune-eszközök problémáinak elhárítása

Most a probléma megoldásához kövesse az alább felsorolt erőforrások áttekintése. 
  
Néhány gyakori hibaüzenetek és a megoldás lépéseit:
  
 **Nem lehet telepíteni a szoftvert, 0x80cf4017:** A fiók-tanúsítvány lejárt. Töltse le újra a PC-ügyfél szoftvercsomag Intune felügyeleti konzolon. Tekintse át a dokumentációjában talál további információt. 
  
 **0x801c0003 hibakód:** A hiba akkor fordulhat elő, az alábbi esetekben: 
  
1. A felhasználó rendelkezik az eszköz által megszabott mint igényelt további eszközöket. Tekintse át [az eszköz eltávolítása](https://docs.microsoft.com/intune/devices-wipe) vagy [módosítása az eszköz által megszabott](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)e dokumentumokat.
    
2. "Felhasználó csatlakozhat egy eszközök Azure ad" "nincs" értékre van állítva. Állítsa be az összes, vagy válassza ki a felhasználók. [Ez a dokumentáció](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) áttekintése. 
    
3. Az eszköz egy másik felhasználó már részesül. Ez a helyzet, ha az eszköz eltávolítása a Azure Intune konzolról vagy kézzel unenroll az eszköz ismételt próbálkozás előtt.
    
4. Az eszköz Windows 10 Home. Csak Windows 10 Pro, oktatási és vállalati SKU Azure Active Directory csatlakozhat.
    
A probléma megoldásához további erőforrások:
  
1. [Intune hibaelhárítás Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) segítségével azonosíthatja és megoldhatja a beiktatási gyakori hibák. [Ez a dokumentum](https://docs.microsoft.com/intune/help-desk-operators) további részletekért tekintse át. 
    
2. Tekintse át ezeket a dokumentumokat, amelyek megakadályozzák a tanúsítványigénylési és -megoldások egyes gyakori hibák listája: [Útmutató a hibaelhárítás](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) és a [Hibaelhárítás doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Útmutató a Windows Microsoft Intune eszközök igénylésére](https://docs.microsoft.com/intune/windows-enroll).
  

