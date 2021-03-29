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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403745"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="0dc8a-102">Nem indul el a munkafolyamat</span><span class="sxs-lookup"><span data-stu-id="0dc8a-102">Workflow is not starting</span></span>

- <span data-ttu-id="0dc8a-103">A SharePoint 2010-es és a SharePoint 2013-as munkafolyamatok nem indulnak el.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="0dc8a-104">Ha a munkafolyamat nem indul el, átmeneti szolgáltatás-probléma lehet, amely miatt a felhasználók időnként késéseket tapasztalhatnak a munkafolyamat előrehaladásával.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="0dc8a-105">Ellenőrizze a [Szolgáltatás állapota irányítópulton,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) hogy nincs-e hatással a szervezete.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="0dc8a-106">Ha a probléma első jelentkezte óta több mint 24 óra telt el, kérjük, írjon be egy támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="0dc8a-107">Sok esetben már dolgozunk a megoldáson.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="0dc8a-108">Kérjük, várjon legalább 24 órát a megoldásunkra.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="0dc8a-109">A SharePoint 2010-munkafolyamatok késleltetve vannak az indítás során.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="0dc8a-110">Ez akkor fordul elő, ha a munkafolyamatot nagy kötegek indítják el.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="0dc8a-111">(ha például egyszerre több elemet ad hozzá).</span><span class="sxs-lookup"><span data-stu-id="0dc8a-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="0dc8a-112">A munkafolyamatok nem valós idejű futtatásra vannak tervezve, ezért a késés szándékos működés.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="0dc8a-113">Ha a Munkafolyamat összetett Extensible Object Markup Language (XALBUM), az összeállítás lassú lehet.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="0dc8a-114">Ellenőrizze [ezt a](https://support.microsoft.com//kb/3043697) cikket.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="0dc8a-115">Egyszerűsítse vagy tervezse újra a munkafolyamatot a Microsoft SharePoint 2013 munkafolyamat-platformtípusának használatával.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="0dc8a-116">Ha a munkafolyamat előzményei egyre nagyobbak, előfordulhat, hogy véglegesen szeretné véglegesen létrehozni az elemeket, vagy új előzményeket szeretne létrehozni.</span><span class="sxs-lookup"><span data-stu-id="0dc8a-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="0dc8a-117">További információ: [Munkafolyamat előzményeinek végleges végleges módosítása](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="0dc8a-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="0dc8a-118">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="0dc8a-118">Related topics</span></span>
<span data-ttu-id="0dc8a-119">Szeretné kipróbálni a Microsoft Flow-t a SharePoint Online-ban?</span><span class="sxs-lookup"><span data-stu-id="0dc8a-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="0dc8a-120">Folyamat létrehozása</span><span class="sxs-lookup"><span data-stu-id="0dc8a-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="0dc8a-121">SharePoint és Flow</span><span class="sxs-lookup"><span data-stu-id="0dc8a-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
