---
title: Hiányzó munkafolyamat-aktiválás nem sikerült
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36753798"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="1865d-102">Hiányzó munkafolyamat-aktiválás nem sikerült</span><span class="sxs-lookup"><span data-stu-id="1865d-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="1865d-103">Microsoft SharePoint-webhelycsoportban listához vagy tárhoz nem adhat globálisan újrafelhasználható munkafolyamatot (például "jóváhagyás-SharePoint 2010").</span><span class="sxs-lookup"><span data-stu-id="1865d-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="1865d-104">A probléma megoldásához hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="1865d-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="1865d-105">Nyissa meg a webhelycsoport gyökérwebhelyét a SharePoint Designer 2013 alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="1865d-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="1865d-106">A **Webhelyobjektumok**területen válassza a **munkafolyamatok**témakört.</span><span class="sxs-lookup"><span data-stu-id="1865d-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="1865d-107">A **munkafolyamat** -szalag **új** szakaszában válassza az **újból felhasználható munkafolyamat**-t.</span><span class="sxs-lookup"><span data-stu-id="1865d-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="1865d-108">Az **újrahasználható munkafolyamat létrehozása** űrlapon adja meg a \* \* *Repair2010* \* \* nevet.</span><span class="sxs-lookup"><span data-stu-id="1865d-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="1865d-109">A **Platformtípus**lapon kattintson a **SharePoint 2010 munkafolyamat**elemre, majd kattintson **az OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="1865d-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="1865d-110">A **munkafolyamat** -szalag **Mentés** szakaszában válassza a **Közzététel**.</span><span class="sxs-lookup"><span data-stu-id="1865d-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="1865d-111">A **munkafolyamat** menüszalagjának **kezelés** szakaszában jelölje ki a **globálisan közzéteszi**választógombot.</span><span class="sxs-lookup"><span data-stu-id="1865d-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="1865d-112">A megerősítést kérő párbeszédpanelen kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="1865d-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="1865d-113">A webböngészőben keresse meg a webhelycsoport gyökérwebhelyét, és kattintson a **webhelybeállítások** \> webhelycsoport- **szolgáltatásainak**elérésére.</span><span class="sxs-lookup"><span data-stu-id="1865d-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="1865d-114">Majd a **munkafolyamatok** funkció váltása:</span><span class="sxs-lookup"><span data-stu-id="1865d-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="1865d-115">· Ha a szolgáltatás *aktiválva* van, kattintson az **inaktiválás elemre,** majd kattintson az **aktiválás**lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="1865d-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="1865d-116">· Ha a szolgáltatás *inaktív* , kattintson az **aktiválás**gombra.</span><span class="sxs-lookup"><span data-stu-id="1865d-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="1865d-117">További információért olvassa el a következő [cikket](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="1865d-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

