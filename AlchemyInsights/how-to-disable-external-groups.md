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
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704130"
---
# <a name="how-to-disable-external-groups"></a>A külső csoportok letiltása

Külső Yammer: az Exchange átviteli szabályait (ETR), a proaktív vezérlők halmazát, amelyekkel megakadályozhatja, hogy a vállalati adatok meg legyenek osztva. Ha korlátozni szeretné, hogy a felhasználók külső csoportokat hozzanak létre, be kell állítania egy Exchange átviteli szabályt (ETR), majd konfigurálnia kell a Yammer, hogy az Exchange átviteli szabály segítségével tiltsa le a külső üzenetküldést.
  
Miután létrehozott egy szabályt az Exchange Online felügyeleti központban, az alábbi lépésekkel állíthatja be az ETR-t a Yammer alkalmazásban:
  
- Jelentkezzen be a Yammer igazolt rendszergazdaként, és a **Yammer felügyeleti központban**lépjen a C **tartalom és biztonsági beállítások lapra \> .**

- A **külső üzenetkezelés**csoportban jelölje be **az Exchange Online Exchange-átviteli szabályok (ETR) érvényesítése az Yammer-on** című témakört.

- Válassza a **Mentés** gombot.

További információt a [külső üzenetküldés letiltása Yammer-hálózatban](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)című témakörben talál.
  