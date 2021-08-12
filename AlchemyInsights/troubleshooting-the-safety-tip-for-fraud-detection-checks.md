---
title: A csalások biztonsági tipp hibák észlelésére vonatkozó hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955968"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>A csalások biztonsági tipp hibák észlelésére vonatkozó hibák elhárítása

Ha egy olyan üzenet jelenik biztonsági tipp, hogy "A feladó nem sikerült a csalás észlelésére vonatkozó ellenőrzéseket végezni, és előfordulhat, hogy nem az, akinek látszik", akkor a feladó nem tudta átadni a DKIM vagy az SPF hitelesítési ellenőrzést. A probléma megoldásának legjobb módja, ha a feladónak engedélyeznie kell magát. Ha a feladó az Ön nevében küld üzenetet, engedélyeznie kell azt úgy, hogy hozzáadja a feladó IP-címét az SPF rekordhoz.
  
További [információt A vörös (gyanús) biztonsági tipp hibák elhárítása a csalás](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) észleléséhez témakörben.
  
Íme néhány további hivatkozás, amely segíthet:
  
- [Hogyan használja a Microsoft a feladói házirend keretrendszerét (SPF) a hamisítás megelőzéséhez?](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF beállítása a hamisítás megelőzéséhez](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
