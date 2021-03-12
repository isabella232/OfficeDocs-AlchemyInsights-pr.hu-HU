---
title: Ajánlott eljárások alkalmazása speciális keresési lekérdezésekhez
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746183"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="ec3ea-102">Ajánlott eljárások alkalmazása speciális keresési lekérdezésekhez</span><span class="sxs-lookup"><span data-stu-id="ec3ea-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="ec3ea-103">Az alábbi ajánlott eljárásokat alkalmazva gyorsabban és elkerülheti az időtúllépéseket az összetett lekérdezések futtatásakor:</span><span class="sxs-lookup"><span data-stu-id="ec3ea-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="ec3ea-104">Amikor új lekérdezéseket próbál ki, mindig korlátot használjon, hogy elkerülje a rendkívül nagy méretű találatkészletek be- vagy kiesését.</span><span class="sxs-lookup"><span data-stu-id="ec3ea-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="ec3ea-105">Az eredményhalmaz méretének előzetes felmérésére `count` is használható.</span><span class="sxs-lookup"><span data-stu-id="ec3ea-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="ec3ea-106">Először használjon időszűrőket.</span><span class="sxs-lookup"><span data-stu-id="ec3ea-106">Use time filters first.</span></span> <span data-ttu-id="ec3ea-107">Ideális esetben csak hét napra korlátozza a lekérdezéseket.</span><span class="sxs-lookup"><span data-stu-id="ec3ea-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="ec3ea-108">A lekérdezés elején, közvetlenül az időszűrő után vegye fel azokat a szűrőket, amelyek várhatóan eltávolítják a legtöbb adatot.</span><span class="sxs-lookup"><span data-stu-id="ec3ea-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="ec3ea-109">Teljes jogkivonatok keresve a helyett `has` használja az `contains` operátort.</span><span class="sxs-lookup"><span data-stu-id="ec3ea-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="ec3ea-110">Nem minden oszlopban, hanem egy adott oszlopon futtathat keresést.</span><span class="sxs-lookup"><span data-stu-id="ec3ea-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="ec3ea-111">Táblázatok egyesolása esetén először adja meg azt a táblázatot, amely kevesebb sort tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="ec3ea-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="ec3ea-112">`project` csak a szükséges oszlopokat a összekapcsolt táblázatokból.</span><span class="sxs-lookup"><span data-stu-id="ec3ea-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="ec3ea-113">További információt a Speciális keresési [lekérdezési gyakorlati tanácsok .](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="ec3ea-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
