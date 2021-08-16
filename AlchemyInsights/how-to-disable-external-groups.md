---
title: A külső csoportok letiltása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015622"
---
# <a name="how-to-disable-external-groups"></a>A külső csoportok letiltása

Yammer külső üzenetküldést Exchange átviteli szabályok ( EETR-k) – olyan proaktív vezérlők halmaza, amelyek megakadályozzák a céges adatok megosztott voltát. Ahhoz, hogy a felhasználók ne hoz tudjanak létre külső csoportokat, konfigurálnia kell egy Exchange átviteli szabályt (ETR), majd úgy kell konfigurálnia az Yammer-t, hogy az Exchange átviteli szabály letiltsa a külső üzenetküldést.
  
Miután létrehozott egy szabályt a Exchange Online felügyeleti központban, az alábbi lépéseket követve állítsa be az ETR alkalmazását a Yammer:
  
- Jelentkezzen be a Yammer rendszergazdaként, és a **Yammer Felügyeleti központban** lépjen a C tartalom- és biztonsági biztonsági beállítások **\> Gépház.**

- A **Külső üzenetküldés alatt jelölje** be A saját Exchange Online Exchange **(EETR-k) érvényesítése) jelölőnégyzetet a Yammer.**

- Válassza a **Mentés** gombot.

További információ: Külső üzenetküldés letiltása Yammer [hálózaton.](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  