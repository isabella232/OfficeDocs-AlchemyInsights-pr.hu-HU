---
title: A csalások észlelését ellenőrző biztonsági tippek hibaelhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658412"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>A csalások észlelését ellenőrző biztonsági tippek hibaelhárítása

Ha olyan biztonsági tippet kap, amely azt mondja, hogy "a feladó nem tudta a csalás észlelési vizsgálatát, és nem lehet, hogy kik jelennek meg", akkor a feladó nem tudta átadni a DKIM vagy az SPF-hitelesítési ellenőrzéseket. A legjobb megoldás, ha a feladónak engedélyezni szeretné a feladót. Ha a feladó az Ön nevében küldi el a feladót, engedélyeznie kell őket úgy, hogy hozzáadja a feladó IP-címét az SPF rekordhoz.
  
További információért olvassa el [a hibák elhárítása a vörös (gyanús) biztonsági tippekkel](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) című témakört.
  
Íme néhány további hivatkozás, amelyek segítséget nyújthatnak:
  
- [Hogyan használja a Microsoft a feladói házirend keretrendszert (SPF) a hamisítás megakadályozására](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Az SPF beállítással megakadályozhatja a hamisítást](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
