---
title: Élő események létrehozásával kapcsolatos hibák a Yammerben
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: eb1ef3712038827beafc8eb520f9793da5f357d728e8250c16d88a99b8b5fe20
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114930"
---
# <a name="live-events-in-yammer-creation-errors"></a>Élő események létrehozásával kapcsolatos hibák a Yammerben

**Élő esemény létrehozása a Yammerben**

A Yammer minden alkalommal megjeleníti az élő esemény létrehozására szolgáló lehetőséget. Egyes esetekben a felhasználók nem felelnek meg az élő események létrehozásához szükséges követelményeknek, és a létrehozás megkísérlésekor hibaüzenetet kapnak. Az alábbi elemek jelzik a probléma általános okait, és megoldásokat adnak a végfelhasználók részére.

**Kik hozhatnak létre élő eseményeket?**
- Egy Office 365 nagyvállalati E1, E3 vagy E5 csomagra szóló, illetve Office 365 A3 vagy A5 csomagra szóló licenc.
- Élő események létrehozásának engedélyezése a Microsoft Teams felügyeleti központban.
- Élő események létrehozásának engedélyezése a Microsoft Streamben (külső közvetítési appal vagy eszközzel létrehozott események esetén).
- Teljes csapatbeli tagság a szervezeten belül (nem lehet vendég vagy egy másik szervezet tagja).
- Személyes értekezletek ütemezése, képernyőmegosztás és IP-videomegosztás bekapcsolása a csapatértekezlet-házirendjében.

**Élő esemény létrehozásának házirendjei**

A Yammer az Office 365-ös bérlői fiókban a Streamhez megadott, élő eseményekre vonatkozó házirendeket követi. Alapértelmezés szerint a szervezet összes felhasználója létrehozhat élő eseményt. A rendszergazdák [módosíthatják ezt a beállítást, amely megakadályozhatja, hogy a felhasználók élő eseményeket hozzanak létre](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating). Ha a felhasználók házirenddel kapcsolatos hibát kapnak, fontos ellenőrizni, hogy vannak-e engedélyeik az élő események létrehozására.
