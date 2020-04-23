---
title: Külső csoportok letiltása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720770"
---
# <a name="how-to-disable-external-groups"></a>Külső csoportok letiltása

A Yammer külső üzenetküldése az Exchange transport rules (ETRs) szolgáltatást alkalmazza, amely proaktív vezérlők készlete a vállalati adatok megosztásának megakadályozására. Annak érdekében, hogy a felhasználók ne hozzanak létre külső csoportokat, be kell állítania egy Exchange átviteli szabályt (ETR), majd be kell állítania a Yammert úgy, hogy az Exchange Transport szabályt használja a külső üzenetküldés letiltására.
  
Miután létrehozott egy szabályt az Exchange Online Felügyeleti központban, az alábbi lépésekkel állíthatja be az ETR-t a Yammerben való alkalmazáshoz:
  
- Jelentkezzen be a Yammerbe ellenőrzött rendszergazdaként, és a **Yammer Felügyeleti központban**nyissa meg a C **tartalom- és biztonsági \> biztonsági beállítások at.**

- A **Külső üzenetküldés**csoportban jelölje **be az Exchange Online Exchange átviteli szabályok (ETRs) érvényesítése a Yammerben jelölőnégyzetet.**

- Válassza a **Mentés** gombot.

További információt a [Külső üzenetek letiltása Yammer-hálózatban](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)című témakörben talál.
  