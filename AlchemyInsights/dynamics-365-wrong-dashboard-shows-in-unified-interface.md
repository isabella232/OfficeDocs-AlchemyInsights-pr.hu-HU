---
title: Dynamics 365 – Nem megfelelő irányítópult jelenik meg a Dynamics 365 Egyesített felületen
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101484"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Nem megfelelő irányítópult jelenik meg a Dynamics 365 egyesített felületén

Több oka is lehet annak, ha a várttól eltérő irányítópultot lát:

## <a name="the-user-has-set-a-user-default-dashboard"></a>A felhasználó beállított egy alapértelmezett felhasználói irányítópultot 

Általában akkor tudja azonosítani az alapértelmezett  felhasználói irányítópultot, ha az Alapértelmezett gomb nem látható az irányítópult parancssávján. A felhasználói alapértelmezett irányítópult felülírja az összes többi alapértelmezett irányítópultot, még akkor is, ha a felhasználó alapértelmezett irányítópultja nem az aktuális appban van.

Az alábbi kerülő megoldással megszedheti az alapértelmezett irányítópultot.

1. Hozzon létre egy új személyes irányítópultot.

2. Állítsa be az új irányítópultot alapértelmezettként.

3. Törölje az irányítópultot.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Az irányítópult a webhelytérképen van beállítva

Előfordulhat, hogy egy szervezeti alapértelmezett irányítópultot úgy állíthat be, hogy kijelöl egy irányítópultot, majd a Rendszer testreszabása alatt az "Alapértelmezettként" adatokat választja. A webhelytérkép-tervezőben definiált irányítópult azonban elsőbbséget élvez az irányítópult felett, ha a felhasználó hozzáfér az irányítópulthoz.

Ha azt, hogy a felhasználók az Ön által alapértelmezettként beállított irányítópultot látják, a következőt használhatja:

* Az irányítópult beállítása a webhelytérképen

* A webhelytérkép által definiált irányítópult elérésének eltávolítása az adott felhasználóknál
