---
title: A Dynamics 365-a Dynamics 365-ban az egyesített felületen nem jelenik meg a megfelelő irányítópult
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711277"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Helytelen irányítópult-bemutató a Dynamics 365 egyesített felületén

Több oka lehet annak, ha a várttól eltérő irányítópult jelenik meg:

## <a name="the-user-has-set-a-user-default-dashboard"></a>A felhasználó beállított egy felhasználó alapértelmezett irányítópultot 

Általában akkor lehet megállapítani, ha a felhasználó alapértelmezett irányítópultja van beállítva, ha a **Beállítás alapértelmezettként** gomb nem jelenik meg az irányítópult-parancssorban. A felhasználó alapértelmezett irányítópultja felülírja az összes többi alapértelmezett irányítópultot, még akkor is, ha a felhasználó alapértelmezett irányítópultja nem szerepel az aktuális alkalmazásban.

Az alapértelmezett irányítópult törléséhez használja az alábbi kerülő megoldást.

1. Hozzon létre egy új személyes irányítópultot.

2. Állítsa be az új irányítópultot alapértelmezettként.

3. Törölje az irányítópultot.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Az irányítópult a webhelytérképben van beállítva

Lehet, hogy a szervezet alapértelmezett irányítópultját egy irányítópult kijelölésével, majd a "rendszer testreszabása" elemre kattintva választhatja ki. A webhelytérkép-tervezőben definiált irányítópult azonban előnyben részesíti az irányítópultot, ha a felhasználó hozzáféréssel rendelkezik.

Ha azt szeretné, hogy a felhasználók a szervezeti alapértelmezettként beállított irányítópultot lássák, az alábbiakat teheti:

* Az irányítópult beállítása a webhelytérképben

* A webhelytérképhez meghatározott irányítópult elérésének megszüntetése a felhasználóknak
