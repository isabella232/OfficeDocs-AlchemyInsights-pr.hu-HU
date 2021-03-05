---
title: Az Exchange Server biztonsági frissítéseit
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481953"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="6155e-102">Az Exchange Server biztonsági frissítéseit</span><span class="sxs-lookup"><span data-stu-id="6155e-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="6155e-103">A Microsoft számos kritikus biztonsági frissítést adott ki a helyszíni Exchange Serverhez.</span><span class="sxs-lookup"><span data-stu-id="6155e-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="6155e-104">Az érintett kiszolgálóverziók az Exchange Server 2010, 2013, 2016 és 2019 frissítési szintjei.</span><span class="sxs-lookup"><span data-stu-id="6155e-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="6155e-105">Az Exchange Online-t nem befolyásolja, de ha a hibrid konfiguráció miatt vannak helyszíni Exchange-kiszolgálói, azok potenciálisan védtelenek.</span><span class="sxs-lookup"><span data-stu-id="6155e-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="6155e-106">A helyszíni kiszolgálók frissítéséhez legalább az alábbi Exchange-verzióknak kell futnia:</span><span class="sxs-lookup"><span data-stu-id="6155e-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="6155e-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="6155e-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="6155e-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="6155e-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="6155e-109">Exchange Server 2016 CU 19 vagy CU 18</span><span class="sxs-lookup"><span data-stu-id="6155e-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="6155e-110">Exchange Server 2019 CU 8 vagy CU 7</span><span class="sxs-lookup"><span data-stu-id="6155e-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="6155e-111">Kérjük, olvassa el a következő közleményt a javítások helyéről: [Megjelent: 2021. márciusi Exchange Server biztonsági frissítések](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="6155e-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="6155e-112">**Fontos megjegyzések:**</span><span class="sxs-lookup"><span data-stu-id="6155e-112">**Important notes:**</span></span>

<span data-ttu-id="6155e-113">A frissítések telepítése nem fog működni, ha a helyszíni kiszolgálók nem futtatják a szükséges Exchange-verziókat a fenti listában láthatóak szerint.</span><span class="sxs-lookup"><span data-stu-id="6155e-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="6155e-114">Ha manuálisan telepíti a frissítéseket, fontos információkért olvassa el a tudásbáziscikkek "Ismert problémák" című szakaszát.</span><span class="sxs-lookup"><span data-stu-id="6155e-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="6155e-115">A biztonsági frissítéseket emelt szintű CMD/PowerShell-parancssorból kell futtatni.</span><span class="sxs-lookup"><span data-stu-id="6155e-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
