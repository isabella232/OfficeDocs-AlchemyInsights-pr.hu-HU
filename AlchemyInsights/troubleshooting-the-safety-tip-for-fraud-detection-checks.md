---
title: A csalás észlelésével kapcsolatos biztonsági tipp hibaelhárítása
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834733"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>A csalás észlelésével kapcsolatos biztonsági tipp hibaelhárítása

Ha egy biztonsági tipp jelenik meg arról, hogy "A feladó nem sikerült a csalás észlelésére vonatkozó ellenőrzéseket végezni, és előfordulhat, hogy nem az, akinek kikiált", akkor a feladó nem tudta átadni a DKIM vagy az SPF hitelesítési ellenőrzéseket. A probléma megoldásának legjobb módja, ha a feladónak engedélyeznie kell magát. Ha a feladó az Ön nevében küld üzenetet, engedélyeznie kell azt úgy, hogy hozzáadja a feladó IP-címét az SPF rekordhoz.
  
További [információt A vörös (gyanús) biztonsági](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) tipp hibaelhárítása csalás észleléséhez témakörben kaphat.
  
Íme néhány további hivatkozás, amely segíthet:
  
- [Hogyan használja a Microsoft a feladói házirend keretrendszerét (SPF) a hamisítás megelőzéséhez?](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF beállítása a hamisítás megelőzéséhez](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
