---
title: A diagram különböző számú rekordot jelenít meg a rácsban
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439354"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>A diagram különböző számú rekordot jelenít meg a rácsban

**Tünet**

A diagram műszerfal oldalon, ha rákattint a diagram "..." és kattintson a "Rekordok megtekintése", akkor keresse meg a rács oldalon, hogy az összes rekordot. Néha megváltozik a rekordok száma.

**A probléma oka**

Ennek oka az eredeti irányítópult-oldalon lévő diagram és a rács kezdőlapján lévő diagram közötti nézetkülönbség.  

**Megoldás**

1. Ellenőrizze az eredeti oldal nézetét és a rács nézetét, és ellenőrizze, hogy különböznek-e.
2. Módosítsa a rács nézetét úgy, hogy az megfeleljen az eredeti oldal nézetének.
3. Ha a megfelelő nézet nem található, az általában azt jelenti, hogy a nézet nincs engedélyezve az alkalmazástervezőben.
4. Nyissa meg az adott alkalmazás alkalmazástervezőjét, válassza ki az entitást és annak nézeteit, ellenőrizze az engedélyezni, menteni, közzétenni és bezárni kívánt nézetet.
5. Frissítse a lapot.