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
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="b07e6-102">Gyakorlati tanácsok alkalmazása speciális keresési lekérdezésekhez</span><span class="sxs-lookup"><span data-stu-id="b07e6-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="b07e6-103">Az eredmények gyorsabb elérése és az időtúllépések elkerülése érdekében összetett lekérdezések futtatásakor alkalmazza az alábbi ajánlott eljárásokat:</span><span class="sxs-lookup"><span data-stu-id="b07e6-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="b07e6-104">Új lekérdezések kipróbálásakor mindig használjon korlátot, hogy ne legyen rendkívül nagy eredményhalmaz.</span><span class="sxs-lookup"><span data-stu-id="b07e6-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="b07e6-105">Emellett az eredményhalmaz méretének kezdeti felmérésére is `count` használható.</span><span class="sxs-lookup"><span data-stu-id="b07e6-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="b07e6-106">Először használjon időszűrőket.</span><span class="sxs-lookup"><span data-stu-id="b07e6-106">Use time filters first.</span></span> <span data-ttu-id="b07e6-107">A legjobb megoldás, ha a lekérdezéseket hét napra korlátozza.</span><span class="sxs-lookup"><span data-stu-id="b07e6-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="b07e6-108">A lekérdezés elején, közvetlenül az időszűrő után vegye fel azokat a szűrőket, amelyek várhatóan eltávolítják a legtöbb adatot.</span><span class="sxs-lookup"><span data-stu-id="b07e6-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="b07e6-109">Ha teljes jogkivonatokat keres, ne az `has` operátort, hanem az operátort `contains` használja.</span><span class="sxs-lookup"><span data-stu-id="b07e6-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="b07e6-110">A keresést nem az összes oszlopban, hanem egy adott oszlopban futtatja.</span><span class="sxs-lookup"><span data-stu-id="b07e6-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="b07e6-111">Táblázatok egyeslve először adja meg azt a táblázatot, amely kevesebb sort tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="b07e6-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="b07e6-112">`project` csak az összekapcsolt táblázatok szükséges oszlopai.</span><span class="sxs-lookup"><span data-stu-id="b07e6-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="b07e6-113">További információt a speciális keresési [lekérdezési gyakorlati tanácsokban olvashat.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="b07e6-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
