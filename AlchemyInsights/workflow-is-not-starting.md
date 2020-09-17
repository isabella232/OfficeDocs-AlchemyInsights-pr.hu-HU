---
title: Nem indul el a munkafolyamat
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794769"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="ea578-102">Nem indul el a munkafolyamat</span><span class="sxs-lookup"><span data-stu-id="ea578-102">Workflow is not starting</span></span>

- <span data-ttu-id="ea578-103">A SharePoint 2010 és a SharePoint 2013-munkafolyamatok nem indulnak el.</span><span class="sxs-lookup"><span data-stu-id="ea578-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="ea578-104">Ha a munkafolyamata nem indul el, lehet, hogy ideiglenes szolgáltatási problémát tapasztal, ahol a felhasználók időnként késleltetni fogják a munkafolyamatok állapotát.</span><span class="sxs-lookup"><span data-stu-id="ea578-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="ea578-105">A [szolgáltatás állapota irányítópulton](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) ellenőrizheti, hogy a szervezete hatással van-e rá.</span><span class="sxs-lookup"><span data-stu-id="ea578-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="ea578-106">Ha több mint 24 óra telt el, mióta először látta ezt a problémát, kérjük, jelentkezzen be egy támogatási jegybe.</span><span class="sxs-lookup"><span data-stu-id="ea578-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="ea578-107">Sok esetben már dolgozunk a megoldáson.</span><span class="sxs-lookup"><span data-stu-id="ea578-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="ea578-108">Kérjük, hogy végezze el a megfelelő megoldást legalább 24 óráig.</span><span class="sxs-lookup"><span data-stu-id="ea578-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="ea578-109">A SharePoint 2010-munkafolyamatai a kezdőképernyőn késleltetve jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="ea578-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="ea578-110">Ez akkor fordul elő, ha a munkafolyamatot nagy kötegekben indítja el.</span><span class="sxs-lookup"><span data-stu-id="ea578-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="ea578-111">(például ha egyszerre több elemet adott meg).</span><span class="sxs-lookup"><span data-stu-id="ea578-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="ea578-112">A munkafolyamatok nem futtathatók valós időben, ezért a késések a tervezés viselkedését szolgálják.</span><span class="sxs-lookup"><span data-stu-id="ea578-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="ea578-113">Ha a munkafolyamat összetett Extensible Object Markup Language (XMOL), a fordítás lassú lehet.</span><span class="sxs-lookup"><span data-stu-id="ea578-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="ea578-114">Olvassa el [ezt a](https://support.microsoft.com//kb/3043697) cikket.</span><span class="sxs-lookup"><span data-stu-id="ea578-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="ea578-115">Egyszerűsíteni kell a munkafolyamatot, vagy át kell terveznie a Microsoft SharePoint 2013 munkafolyamat-platform típusa használatával.</span><span class="sxs-lookup"><span data-stu-id="ea578-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="ea578-116">Ha a munkafolyamat előzményei nagyban nőttek, érdemes lehet törölni az elemeket, vagy létre kell hoznia egy új előzményeket tartalmazó listát.</span><span class="sxs-lookup"><span data-stu-id="ea578-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="ea578-117">További információ: [munkafolyamat-előzmények törlése](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="ea578-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="ea578-118">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="ea578-118">Related topics</span></span>
<span data-ttu-id="ea578-119">Szeretné kipróbálni a Microsoft flow-t a SharePoint Online-ban?</span><span class="sxs-lookup"><span data-stu-id="ea578-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="ea578-120">Folyamatábra létrehozása</span><span class="sxs-lookup"><span data-stu-id="ea578-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ea578-121">SharePoint és flow</span><span class="sxs-lookup"><span data-stu-id="ea578-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


