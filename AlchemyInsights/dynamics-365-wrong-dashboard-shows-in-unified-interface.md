---
title: Dynamics 365 - rossz irányítópult Dynamics 365 egységes felületen látható
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747849"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Rossz irányítópult Dynamics 365 egységes felületen jeleníti meg

Több oka miért várt egy másik irányítópult jelenhetnek meg:

## <a name="the-user-has-set-a-user-default-dashboard"></a>A felhasználó be van állítva az alapértelmezett felhasználói irányítópult 

Általában azonosítani tudja a felhasználót ha az **Alapértelmezett** gomb nem jelenik meg a parancssávon irányítópult beállítása alapértelmezett irányítópultot. Az alapértelmezett felhasználói irányítópult felülírják más alapértelmezett irányítópultok, még akkor is, ha az aktuális alkalmazás nem szerepel a felhasználó alapértelmezett irányítópultot.

Használja az alábbi megoldásokat az Adatbázisjelszó törlése az alapértelmezett irányítópultot.

1. Hozzon létre egy új személyes irányítópult.

2. Ez új irányítópult beállítása a felhasználó alapértelmezett.

3. Adott irányítópult törlése.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Az irányítópult van megadva az Oldaltérkép

Beállított egy szervezet alapértelmezett irányítópultot irányítópult kijelölésével, majd válassza a "Alapértelmezett" "A rendszer testreszabása" alatt. De az irányítópult a webhelytérkép-tervezőben meghatározott elsőbbséget élveznek az irányítópultot, ha a felhasználónak van hozzáférése.

Ahhoz, hogy a felhasználók megtekinthetik a szervezet alapértelmezett beállítása az irányítópultot, közül választhat:

* Az oldaltérkép az adott irányítópult beállítása

* Távolítsa el a felhasználók hozzáférését az Oldaltérkép definiált irányítópulton