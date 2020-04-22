---
title: A munkafolyamat nem indul el
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766099"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="9dd67-102">A munkafolyamat nem indul el</span><span class="sxs-lookup"><span data-stu-id="9dd67-102">Workflow is not starting</span></span>

- <span data-ttu-id="9dd67-103">A SharePoint 2010 és a SharePoint 2013 munkafolyamatai nem indulnak el.</span><span class="sxs-lookup"><span data-stu-id="9dd67-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="9dd67-104">Ha a munkafolyamat nem indul el, előfordulhat, hogy ideiglenes szolgáltatásprobléma merül fel, amelyben a felhasználók időszakos késéseket tapasztalhatnak a munkafolyamat előrehaladásával.</span><span class="sxs-lookup"><span data-stu-id="9dd67-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="9dd67-105">Ellenőrizze a [Szolgáltatásállapot-irányítópulton,](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) hogy a szervezet érintett-e.</span><span class="sxs-lookup"><span data-stu-id="9dd67-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="9dd67-106">Ha több mint 24 óra telt el azóta, hogy először látta ezt a problémát, kérjük, jelentkezzen be egy támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="9dd67-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="9dd67-107">Sok esetben már dolgozunk a megoldáson.</span><span class="sxs-lookup"><span data-stu-id="9dd67-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="9dd67-108">Kérjük, adjon nekünk legalább 24 órát a megoldás befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="9dd67-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="9dd67-109">A SharePoint 2010-munkafolyamatok elhúzódnak az indításkor.</span><span class="sxs-lookup"><span data-stu-id="9dd67-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="9dd67-110">Ez akkor fordul elő, ha a munkafolyamat nagy kötegekben aktiválódik.</span><span class="sxs-lookup"><span data-stu-id="9dd67-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="9dd67-111">(például ha egyszerre több elemet ad hozzá).</span><span class="sxs-lookup"><span data-stu-id="9dd67-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="9dd67-112">A munkafolyamatokat nem valós idejű futtatásra tervezték, így a késleltetés a by-design viselkedése.</span><span class="sxs-lookup"><span data-stu-id="9dd67-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="9dd67-113">Ha a munkafolyamat összetett Extensible Object Markup Language (XMOL), a fordítás lassú lehet.</span><span class="sxs-lookup"><span data-stu-id="9dd67-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="9dd67-114">Ellenőrizze [ezt a](https://support.microsoft.com//kb/3043697) cikket.</span><span class="sxs-lookup"><span data-stu-id="9dd67-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="9dd67-115">Egyszerűsítse a munkafolyamatot, vagy tervezze újra a Microsoft SharePoint 2013 munkafolyamat-platformtípushasználatával.</span><span class="sxs-lookup"><span data-stu-id="9dd67-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="9dd67-116">Ha a munkafolyamat előzményei megnőttek, érdemes lehet kiüríteni az elemeket, vagy új előzménylistát létrehozni.</span><span class="sxs-lookup"><span data-stu-id="9dd67-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="9dd67-117">További információ : [A munkafolyamat előzményeinek törlése](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="9dd67-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="9dd67-118">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="9dd67-118">Related topics</span></span>
<span data-ttu-id="9dd67-119">Kiszeretné próbálni a Microsoft Flow-t a SharePoint Online-ban?</span><span class="sxs-lookup"><span data-stu-id="9dd67-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="9dd67-120">Folyamat létrehozása</span><span class="sxs-lookup"><span data-stu-id="9dd67-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="9dd67-121">SharePoint és Folyamat</span><span class="sxs-lookup"><span data-stu-id="9dd67-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


