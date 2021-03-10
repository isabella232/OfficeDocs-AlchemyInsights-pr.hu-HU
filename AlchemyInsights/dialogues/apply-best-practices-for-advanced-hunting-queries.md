---
title: Gyakorlati tanácsok alkalmazása speciális keresési lekérdezésekhez
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694272"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Gyakorlati tanácsok alkalmazása speciális keresési lekérdezésekhez

Az eredmények gyorsabb elérése és az időtúllépések elkerülése érdekében összetett lekérdezések futtatásakor alkalmazza az alábbi ajánlott eljárásokat:

- Új lekérdezések kipróbálásakor mindig használjon korlátot, hogy ne legyen rendkívül nagy eredményhalmaz. Emellett az eredményhalmaz méretének kezdeti felmérésére is `count` használható.
- Először használjon időszűrőket. A legjobb megoldás, ha a lekérdezéseket hét napra korlátozza.
- A lekérdezés elején, közvetlenül az időszűrő után vegye fel azokat a szűrőket, amelyek várhatóan eltávolítják a legtöbb adatot.
- Ha teljes jogkivonatokat keres, ne az `has` operátort, hanem az operátort `contains` használja.
- A keresést nem az összes oszlopban, hanem egy adott oszlopban futtatja.
- Táblázatok egyeslve először adja meg azt a táblázatot, amely kevesebb sort tartalmaz.
- `project` csak az összekapcsolt táblázatok szükséges oszlopai.

További információt a speciális keresési [lekérdezési gyakorlati tanácsokban olvashat.](https://go.microsoft.com/fwlink/?linkid=2144812)
