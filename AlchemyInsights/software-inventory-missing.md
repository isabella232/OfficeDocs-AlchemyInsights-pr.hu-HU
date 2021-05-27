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
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="c1fc3-102">A szoftverkészlet hiányzik vagy pontatlan</span><span class="sxs-lookup"><span data-stu-id="c1fc3-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="c1fc3-103">A Veszélyforrás- és biztonságirés-kezelés (TVM) szoftverkészlete a szervezetben hivatalos közös platform-számokkal (CPE) együtt ismert szoftverek listája.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="c1fc3-104">A hivatalos CPE-hez nem kötött szoftvertermékekhez nem jelentek meg biztonsági rések.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="c1fc3-105">A készlet olyan adatokat is tartalmaz, mint például a szállító neve, a veszélyforrások száma, a veszélyforrások és a felfedett eszközök száma.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="c1fc3-106">Az eszközökön végrehajtott szoftverváltozások általában két órán belül jelennek meg a biztonsági portálon.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="c1fc3-107">Időnként azonban tovább is tarthat.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="c1fc3-108">Jelenleg nem lehet kényszeríteni a szinkronizálást; ez egy folyamatos felmérés.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="c1fc3-109">Ha a szoftver módosítása esetén a módosítás 5 óra múlva nem jelenik meg megfelelően a TVM-ben, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="c1fc3-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="c1fc3-110">A szoftver észlelésének ellenőrzéséhez tekintse meg a szoftver bizonyítékokat és szoftvereket bizonyító szakaszát.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="c1fc3-111">Győződjön meg arról, hogy a szoftver támogatott.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-111">Make sure that the software is supported.</span></span> <span data-ttu-id="c1fc3-112">Előfordulhat, hogy a szoftver csak az eszköz szintjén látható, még akkor is, ha a felhasználó jelenleg nem Veszélyforrás- és biztonságirés-kezelés.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="c1fc3-113">Azonban csak korlátozott adatok érhetők el.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="c1fc3-114">Az inaccuracy jelentéséhez a portálról való jelentés lépéseit az [Inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)jelentése oldalon láthatja.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="c1fc3-115">**Megjegyzés:** A pontatlanság jelentése az MDE portálról egy egycsatornás csatornát jelent a tervezéshez.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="c1fc3-116">Ha a probléma sürgős, nyisson egy támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="c1fc3-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="c1fc3-117">További információ: [Szoftverkészlet – Veszélyforrás- és biztonságirés-kezelés.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)</span><span class="sxs-lookup"><span data-stu-id="c1fc3-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>