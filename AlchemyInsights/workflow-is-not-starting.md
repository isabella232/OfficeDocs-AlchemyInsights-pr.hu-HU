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
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738091"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="665a7-102">A munkafolyamat nem indul</span><span class="sxs-lookup"><span data-stu-id="665a7-102">Workflow is not starting</span></span>

- <span data-ttu-id="665a7-103">Nem indul el a SharePoint 2010 és a SharePoint 2013 munkafolyamatok.</span><span class="sxs-lookup"><span data-stu-id="665a7-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="665a7-104">Ha a munkafolyamat nem indul el, előfordulhat, hogy ideiglenes szolgáltatási probléma áll fenn, ahol a felhasználók időszakos késleltetést tapasztalhatnak a munkafolyamat előrehaladása során.</span><span class="sxs-lookup"><span data-stu-id="665a7-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="665a7-105">Ellenőrizze a [szolgáltatás Állapotirányítópultját](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , hogy a szervezet hatással van-e rá.</span><span class="sxs-lookup"><span data-stu-id="665a7-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="665a7-106">Ha több mint 24 óra telt el mióta először meglátta ezt a problémát, kérjük, jelentkezzen be a támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="665a7-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="665a7-107">Sok esetben már dolgozunk a megoldásban.</span><span class="sxs-lookup"><span data-stu-id="665a7-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="665a7-108">Kérjük, hogy a megoldás befejezéséhez legalább 24 órát adjon nekünk.</span><span class="sxs-lookup"><span data-stu-id="665a7-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="665a7-109">Az indulva késleltetett SharePoint 2010-munkafolyamatok.</span><span class="sxs-lookup"><span data-stu-id="665a7-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="665a7-110">Ez akkor fordulhat elő, ha a munkafolyamatot nagyméretű kötegekben indítja el.</span><span class="sxs-lookup"><span data-stu-id="665a7-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="665a7-111">(például több elem egyidejű hozzáadása esetén).</span><span class="sxs-lookup"><span data-stu-id="665a7-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="665a7-112">A munkafolyamatokat nem úgy tervezték, hogy valós idejű fusson, így a késés a tervezéssel szemben.</span><span class="sxs-lookup"><span data-stu-id="665a7-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="665a7-113">Ha a munkafolyamat összetett bővíthető Objektumleíró nyelv (XMOL), a fordítás lassú lehet.</span><span class="sxs-lookup"><span data-stu-id="665a7-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="665a7-114">Ellenőrizze [ezt a](https://support.microsoft.com//kb/3043697) cikket.</span><span class="sxs-lookup"><span data-stu-id="665a7-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="665a7-115">Egyszerűsítse a munkafolyamatot, vagy újratervezje a Microsoft SharePoint 2013 workflow platformtípus használatával.</span><span class="sxs-lookup"><span data-stu-id="665a7-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="665a7-116">Ha a munkafolyamat előzményei nagynak nőttek, akkor érdemes lehet az elemeket megtisztítani vagy új előzménylistát létrehozni.</span><span class="sxs-lookup"><span data-stu-id="665a7-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="665a7-117">További információk: a [munkafolyamat előzményeinek törlése](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="665a7-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="665a7-118">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="665a7-118">Related topics</span></span>
<span data-ttu-id="665a7-119">Szeretné kipróbálni a Microsoft flow-t a SharePoint Online szolgáltatásban?</span><span class="sxs-lookup"><span data-stu-id="665a7-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="665a7-120">Átfolyás létrehozása</span><span class="sxs-lookup"><span data-stu-id="665a7-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="665a7-121">SharePoint-és adatfolyam</span><span class="sxs-lookup"><span data-stu-id="665a7-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


