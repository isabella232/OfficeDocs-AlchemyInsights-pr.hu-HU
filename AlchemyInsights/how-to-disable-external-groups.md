---
title: Külső csoportok letiltása
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540903"
---
# <a name="how-to-disable-external-groups"></a>Külső csoportok letiltása

Yammer külső üzenetküldő Exchange átviteli szabályok – (ETR), a proaktív vezérlők vállalati adatok megosztását, elkerülésére vonatkozik. Annak érdekében, hogy korlátozza a felhasználók külső csoportok létrehozását, kell konfigurálása az Exchange átviteli szabály (ETR), és állítsa be az Exchange átviteli szabály segítségével blokkolja a külső üzenetküldő Yammer.
  
Exchange Online admin center szabály létrehozása után a következő lépésekkel állítsa be az ETR Yammer alkalmaz:
  
- Bejelentkezés Yammer ellenőrzött admin, és **admin center Yammer**, ugorjon a C **tartalom és a biztonsági \> biztonsági beállításokat.**

- A **Külső üzenetküldő**, válassza a **az Exchange Online Exchange közlekedési szabályok érvényesítése – (ETR) a Yammer.**

- Válassza a **Mentés** gombot.

További tudnivalókért tanulmányozza a [külső üzenetküldő Exchange átviteli szabályok Yammer hálózati vezérlő](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  