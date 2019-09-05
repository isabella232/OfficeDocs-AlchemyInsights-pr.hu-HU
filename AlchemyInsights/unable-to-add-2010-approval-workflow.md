---
title: Nem lehet hozzáadni a 2010 jóváhagyási munkafolyamatot
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748686"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="c3b7f-102">Nem lehet hozzáadni a 2010 jóváhagyási munkafolyamatot</span><span class="sxs-lookup"><span data-stu-id="c3b7f-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="c3b7f-103">Microsoft SharePoint-webhelycsoportban listához vagy tárhoz nem adhat globálisan újrafelhasználható munkafolyamatot (például "jóváhagyás-SharePoint 2010").</span><span class="sxs-lookup"><span data-stu-id="c3b7f-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="c3b7f-104">A probléma megoldásához hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="c3b7f-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="c3b7f-105">Nyissa meg a webhelycsoport gyökérwebhelyét a SharePoint Designer 2013 alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="c3b7f-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="c3b7f-106">A **Webhelyobjektumok**területen válassza a **munkafolyamatok**témakört.</span><span class="sxs-lookup"><span data-stu-id="c3b7f-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="c3b7f-107">A **munkafolyamat** -szalag **új** szakaszában válassza az **újból felhasználható munkafolyamat**-t.</span><span class="sxs-lookup"><span data-stu-id="c3b7f-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="c3b7f-108">Az **újrahasználható munkafolyamat létrehozása** űrlapon adja meg a \* \* *Repair2010* \* \* nevet.</span><span class="sxs-lookup"><span data-stu-id="c3b7f-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="c3b7f-109">A **Platformtípus**lapon kattintson a **SharePoint 2010 munkafolyamat**elemre, majd kattintson **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="c3b7f-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="c3b7f-110">A **munkafolyamat** -szalag **Mentés** szakaszában válassza a **Közzététel**.</span><span class="sxs-lookup"><span data-stu-id="c3b7f-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="c3b7f-111">A **munkafolyamat** menüszalagjának **kezelés** szakaszában jelölje ki a **globálisan közzéteszi**választógombot.</span><span class="sxs-lookup"><span data-stu-id="c3b7f-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="c3b7f-112">A megerősítést kérő párbeszédpanelen kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="c3b7f-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="c3b7f-113">A webböngészőben keresse meg a webhelycsoport gyökérwebhelyét, és kattintson a **webhelybeállítások** \> webhelycsoport- **szolgáltatásainak**elérésére.</span><span class="sxs-lookup"><span data-stu-id="c3b7f-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="c3b7f-114">A **munkafolyamatok** funkció váltása:</span><span class="sxs-lookup"><span data-stu-id="c3b7f-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="c3b7f-115">· Ha a szolgáltatás *aktiválva* van, kattintson az **inaktiválás elemre,** majd kattintson az **aktiválás**lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="c3b7f-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="c3b7f-116">· Ha a szolgáltatás *inaktív* , kattintson az **aktiválás**gombra.</span><span class="sxs-lookup"><span data-stu-id="c3b7f-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="c3b7f-117">További információért olvassa el a következő [cikket](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="c3b7f-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

