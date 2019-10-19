---
title: Dynamics 365-hibás irányítópult-műsorok Dynamics 365 egyesített illesztő
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528553"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Hibás irányítópult-bemutatók a Dynamics 365 egységes illesztőfelületen

Több oka is lehet, hogy miért jelenik meg egy másik irányítópult, mint amit elvársz:

## <a name="the-user-has-set-a-user-default-dashboard"></a>A felhasználó beállította a felhasználó alapértelmezett irányítópultját 

Általában akkor lehet azonosítani egy felhasználói alapértelmezett irányítópultot, ha az **alapértelmezés szerinti beállítás** gomb nem jelenik meg az irányítópult parancssávján. A felhasználó alapértelmezett irányítópultja felülírja az összes többi alapértelmezett irányítópultot még akkor is, ha a felhasználó alapértelmezett irányítópultja nem szerepel az aktuális alkalmazásban.

A következő kerülő megoldás segítségével állítsa be az alapértelmezett irányítópultot.

1. Hozzon létre egy új személyes irányítópultot.

2. Az új irányítópult beállítása felhasználói alapértelmezésként.

3. Törölje az irányítópultot.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>A műszerfal van készlet-ban sitemap

Lehet, hogy beállította a szervezet alapértelmezett irányítópultját az irányítópult kijelölésével és a "beállítás alapértelmezettként" választásával a "rendszer testreszabása" címszó alatt. A webhelytérkép-tervezőben definiált irányítópult azonban elsőbbséget élvez az irányítópulttal szemben, ha a felhasználónak hozzáférése van hozzá.

Ha azt szeretné, hogy a felhasználók a szervezet alapértelmezettnek tekintse meg az irányítópultot, az alábbiak közül választhat:

* Az irányítópult beállítása a webhelytérképben

* Távolítsa el a hozzáférést a webhelytérkép definiált irányítópulthoz a felhasználók számára
