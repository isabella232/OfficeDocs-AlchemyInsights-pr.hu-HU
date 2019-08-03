---
title: A munkafolyamat nem indul
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: efd17c302ae6d857207e87e94d74d3794e94a83a
ms.sourcegitcommit: 204be4a6ae03700b75eae6b09b4e9ab283089fbf
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36171787"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="014dc-102">A munkafolyamat nem indul</span><span class="sxs-lookup"><span data-stu-id="014dc-102">Workflow is not starting</span></span>

- <span data-ttu-id="014dc-103">Nem indítja el a SharePoint 2010 és a SharePoint 2013 munkafolyamatok.</span><span class="sxs-lookup"><span data-stu-id="014dc-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    <span data-ttu-id="014dc-104">A munkafolyamat nem indul el, ha lehet egy ideiglenes szolgáltatást a probléma adott felhasználók esetében szakaszos késlekedések tapasztalhatók a munkafolyamat előrehaladását.</span><span class="sxs-lookup"><span data-stu-id="014dc-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="014dc-105">Megtekintheti, ha a szervezet az érintett [Szolgáltatás egészségügyi irányítópult](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) ellenőrizze.</span><span class="sxs-lookup"><span data-stu-id="014dc-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    <span data-ttu-id="014dc-106">24 óránál hosszabb idő telt el azóta, először látta a probléma, ha jelentkezzen egy támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="014dc-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="014dc-107">Sok esetben azt már dolgozik a megoldáson.</span><span class="sxs-lookup"><span data-stu-id="014dc-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="014dc-108">Adja meg a megoldás végrehajtásához legalább 24 órán keresztül.</span><span class="sxs-lookup"><span data-stu-id="014dc-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="014dc-109">SharePoint 2010 munkafolyamatok késleltetett Start.</span><span class="sxs-lookup"><span data-stu-id="014dc-109">SharePoint 2010 workflows delayed on start.</span></span>

    <span data-ttu-id="014dc-110">Ez akkor fordul elő, ha a munkafolyamat elindul a nagy adagok.</span><span class="sxs-lookup"><span data-stu-id="014dc-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="014dc-111">(például, ha több elemekre egyszerre).</span><span class="sxs-lookup"><span data-stu-id="014dc-111">(for example, when several items are added at once).</span></span>

    <span data-ttu-id="014dc-112">A munkafolyamatok futtatása valós idejű, így a késedelem a jelenség tudatos tervezési nem tervezték.</span><span class="sxs-lookup"><span data-stu-id="014dc-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

    <span data-ttu-id="014dc-113">Ha a munkafolyamat összetett bővíthető objektum Markup Language (XMOL), fordítás lassú lehet.</span><span class="sxs-lookup"><span data-stu-id="014dc-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="014dc-114">Ellenőrizze [a](https://support.microsoft.com/en-us/kb/3043697) cikk.</span><span class="sxs-lookup"><span data-stu-id="014dc-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    <span data-ttu-id="014dc-115">A munkafolyamat egyszerűsítése vagy a Microsoft SharePoint 2013 munkafolyamata platform segítségével alakíthatja át.</span><span class="sxs-lookup"><span data-stu-id="014dc-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    <span data-ttu-id="014dc-116">Is ha a munkafolyamat-előzmények nagy nőtt, érdemes az elemek törlése vagy egy új előzménylistát hoz létre.</span><span class="sxs-lookup"><span data-stu-id="014dc-116">Also, if your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

    <span data-ttu-id="014dc-117">További információ: a [munkafolyamat-előzmények törlése](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="014dc-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="014dc-118">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="014dc-118">Related topics</span></span>
<span data-ttu-id="014dc-119">Próbálkozzon a SharePoint Online Microsoft áramlási szeretne?</span><span class="sxs-lookup"><span data-stu-id="014dc-119">Want to try Micrsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="014dc-120">Folyamat létrehozása</span><span class="sxs-lookup"><span data-stu-id="014dc-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="014dc-121">A SharePoint és az áram</span><span class="sxs-lookup"><span data-stu-id="014dc-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


