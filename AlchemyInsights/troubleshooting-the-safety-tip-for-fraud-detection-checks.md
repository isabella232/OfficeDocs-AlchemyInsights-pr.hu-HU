---
title: Hibaelhárítás a biztonsági tipp a csalások felderítése ellenőrzések
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759514"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Hibaelhárítás a biztonsági tipp a csalások felderítése ellenőrzések

Ha olyan biztonsági tippet kap, amely szerint "A feladó megbukott a csalásészlelési ellenőrzéseken, és nem lehet az, akinek látszik", akkor a feladó nem tudta átadni a DKIM vagy az SPF hitelesítési ellenőrzéseket. A megoldás legjobb módja az, ha a feladó engedélyezi magát. Ha a feladó az Ön nevében küld, engedélyeznie kell őket a feladó IP-címének hozzáadásával az SPF-rekordhoz.
  
További információ [a csalásészlelési ellenőrzésekért olvassa el a piros (gyanús) biztonsági tipp hibaelhárítása](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) című témakört.
  
Íme néhány további link, amely segíthet:
  
- [Hogyan használja a Microsoft a feladói házirend keretrendszerét (SPF) a hamisítás megakadályozására?](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Az SPF beállítása a hamisítás megakadályozása érdekében](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
