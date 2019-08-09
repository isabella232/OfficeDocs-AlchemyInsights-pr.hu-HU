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
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270782"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="8502b-102">A munkafolyamat nem indul</span><span class="sxs-lookup"><span data-stu-id="8502b-102">Workflow is not starting</span></span>

- <span data-ttu-id="8502b-103">Nem indítja el a SharePoint 2010 és a SharePoint 2013 munkafolyamatok.</span><span class="sxs-lookup"><span data-stu-id="8502b-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="8502b-104">A munkafolyamat nem indul el, ha lehet egy ideiglenes szolgáltatást a probléma adott felhasználók esetében szakaszos késlekedések tapasztalhatók a munkafolyamat előrehaladását.</span><span class="sxs-lookup"><span data-stu-id="8502b-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="8502b-105">Megtekintheti, ha a szervezet az érintett [Szolgáltatás egészségügyi irányítópult](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) ellenőrizze.</span><span class="sxs-lookup"><span data-stu-id="8502b-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="8502b-106">24 óránál hosszabb idő telt el azóta, először látta a probléma, ha jelentkezzen egy támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="8502b-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="8502b-107">Sok esetben azt már dolgozik a megoldáson.</span><span class="sxs-lookup"><span data-stu-id="8502b-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8502b-108">Adja meg a megoldás végrehajtásához legalább 24 órán keresztül.</span><span class="sxs-lookup"><span data-stu-id="8502b-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="8502b-109">SharePoint 2010 munkafolyamatok késleltetett Start.</span><span class="sxs-lookup"><span data-stu-id="8502b-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="8502b-110">Ez akkor fordul elő, ha a munkafolyamat elindul a nagy adagok.</span><span class="sxs-lookup"><span data-stu-id="8502b-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="8502b-111">(például, ha több elemekre egyszerre).</span><span class="sxs-lookup"><span data-stu-id="8502b-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="8502b-112">A munkafolyamatok futtatása valós idejű, így a késedelem a jelenség tudatos tervezési nem tervezték.</span><span class="sxs-lookup"><span data-stu-id="8502b-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="8502b-113">Ha a munkafolyamat összetett bővíthető objektum Markup Language (XMOL), fordítás lassú lehet.</span><span class="sxs-lookup"><span data-stu-id="8502b-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="8502b-114">Ellenőrizze [a](https://support.microsoft.com/en-us/kb/3043697) cikk.</span><span class="sxs-lookup"><span data-stu-id="8502b-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="8502b-115">A munkafolyamat egyszerűsítése vagy a Microsoft SharePoint 2013 munkafolyamata platform segítségével alakíthatja át.</span><span class="sxs-lookup"><span data-stu-id="8502b-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="8502b-116">Ha a munkafolyamat-előzmények nagy nőtt, célszerű lehet az elemek törlése vagy egy új előzménylistát hoz létre.</span><span class="sxs-lookup"><span data-stu-id="8502b-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="8502b-117">További információ: a [munkafolyamat-előzmények törlése](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="8502b-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="8502b-118">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="8502b-118">Related topics</span></span>
<span data-ttu-id="8502b-119">Próbálkozzon a SharePoint Online Microsoft Flow szeretne?</span><span class="sxs-lookup"><span data-stu-id="8502b-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="8502b-120">Folyamat létrehozása</span><span class="sxs-lookup"><span data-stu-id="8502b-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="8502b-121">A SharePoint és az áram</span><span class="sxs-lookup"><span data-stu-id="8502b-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


