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
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36739495"
---
# <a name="how-to-disable-external-groups"></a>Külső csoportok letiltása

A yammer külső üzenetküldő szolgáltatás az Exchange átviteli szabályokat (ETRs), a vállalati adatok megosztásának megakadályozásához proaktív vezérlőket alkalmaz. Ahhoz, hogy a felhasználók külső csoportokat is létrehozhassák, konfigurálnia kell az Exchange átviteli szabályt (ETR), majd konfigurálnia kell a Yammer programot az Exchange átviteli szabály használatára a külső üzenetek blokkolásához.
  
Miután létrehozott egy szabályt az Exchange Online admin központban, kövesse az alábbi lépéseket az ETR beállításához a Yammer esetében:
  
- Jelentkezzen be Yammer-be ellenőrzött adminisztrátorként, és a **yammer Admin Center**, menjen a C **tartalom-és biztonsági \> beállítások.**

- A **külső üzenetek**területen válassza **az Exchange Online Exchange-átviteli szabályok (Etrs) érvényesítése a yammer-ben.**

- Válassza a **Mentés** gombot.

További információt a [külső üzenetkezelés letiltása Yammer hálózatban](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)című témakörben talál.
  