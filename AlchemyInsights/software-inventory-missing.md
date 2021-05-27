---
title: A szoftverkészlet hiányzik vagy pontatlan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676267"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>A szoftverkészlet hiányzik vagy pontatlan

A Veszélyforrás- és biztonságirés-kezelés (TVM) szoftverkészlete a szervezetben hivatalos közös platform-számokkal (CPE) együtt ismert szoftverek listája.

A hivatalos CPE-hez nem kötött szoftvertermékekhez nem jelentek meg biztonsági rések. A készlet olyan adatokat is tartalmaz, mint például a szállító neve, a veszélyforrások száma, a veszélyforrások és a felfedett eszközök száma.

Az eszközökön végrehajtott szoftverváltozások általában két órán belül jelennek meg a biztonsági portálon. Időnként azonban tovább is tarthat. Jelenleg nem lehet kényszeríteni a szinkronizálást; ez egy folyamatos felmérés.

Ha a szoftver módosítása esetén a módosítás 5 óra múlva nem jelenik meg megfelelően a TVM-ben, kövesse az alábbi lépéseket:

1. A szoftver észlelésének ellenőrzéséhez tekintse meg a szoftver bizonyítékokat és szoftvereket bizonyító szakaszát.
1. Győződjön meg arról, hogy a szoftver támogatott. Előfordulhat, hogy a szoftver csak az eszköz szintjén látható, még akkor is, ha a felhasználó jelenleg nem Veszélyforrás- és biztonságirés-kezelés. Azonban csak korlátozott adatok érhetők el.
1. Az inaccuracy jelentéséhez a portálról való jelentés lépéseit az [Inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)jelentése oldalon láthatja.
   
    **Megjegyzés:** A pontatlanság jelentése az MDE portálról egy egycsatornás csatornát jelent a tervezéshez. Ha a probléma sürgős, nyisson egy támogatási jegyet.

További információ: [Szoftverkészlet – Veszélyforrás- és biztonságirés-kezelés.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)