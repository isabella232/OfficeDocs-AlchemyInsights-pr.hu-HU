---
title: Igénylése a Windows Microsoft Intune-eszközök problémáinak elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665834"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Igénylése a Windows Microsoft Intune-eszközök problémáinak elhárítása

Most a probléma megoldásához kövesse az alább felsorolt erőforrások áttekintése.
  
Néhány gyakori hibaüzenetek és a megoldás lépéseit:
  
 **Nem lehet telepíteni a szoftvert, 0x80cf4017:** A fiók-tanúsítvány lejárt. Töltse le újra a PC-ügyfél szoftvercsomag Intune felügyeleti konzolon. Tekintse át a dokumentációjában talál további információt.
  
 **0x801c0003 hibakód:** A hiba akkor fordulhat elő, az alábbi esetekben:
  
-  A felhasználó rendelkezik az eszköz által megszabott mint igényelt további eszközöket. Tekintse át [az eszköz eltávolítása](https://docs.microsoft.com/intune/devices-wipe) vagy [módosítása az eszköz által megszabott](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)e dokumentumokat.

-  "Felhasználó csatlakozhat egy eszközök Azure ad" értéke "none." Állítsa be az összes, vagy válassza ki a felhasználók. [Ez a dokumentáció](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) áttekintése.

-  Az eszköz egy másik felhasználó már részesül. Ez a helyzet, ha az eszköz eltávolítása a Azure Intune konzolról vagy kézzel unenroll az eszköz ismételt próbálkozás előtt.

-  Az eszköz Windows 10 Home. Csak Windows 10 Pro, oktatási és vállalati SKU Azure Active Directory csatlakozhat.

A probléma megoldásához további erőforrások:
  
-  [Intune hibaelhárítás Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) segítségével azonosíthatja és megoldhatja a beiktatási gyakori hibák. [Ez a dokumentum](https://docs.microsoft.com/intune/help-desk-operators) további részletekért tekintse át.

-  Tekintse át ezeket a dokumentumokat, amelyek megakadályozzák a tanúsítványigénylési és -megoldások egyes gyakori hibák listája: [Útmutató a hibaelhárítás](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) és a [Hibaelhárítás doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Útmutató a Windows Microsoft Intune eszközök igénylésére](https://docs.microsoft.com/intune/windows-enroll).
