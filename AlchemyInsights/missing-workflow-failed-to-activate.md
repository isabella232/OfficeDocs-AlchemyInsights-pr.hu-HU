---
title: Hiányzó munkafolyamat aktiválása sikertelen
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917570"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="0d37d-102">Hiányzó munkafolyamat aktiválása sikertelen</span><span class="sxs-lookup"><span data-stu-id="0d37d-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="0d37d-103">A Microsoft SharePoint-webhelycsoport nem adhat (például a "Jóváhagyás – SharePoint 2010") globálisan újrafelhasználható munkafolyamat listához vagy könyvtárhoz.</span><span class="sxs-lookup"><span data-stu-id="0d37d-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="0d37d-104">A probléma megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="0d37d-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="0d37d-105">Nyissa meg a legfelső szintű webhely helycsoport a SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="0d37d-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="0d37d-106">**A helyobjektumok**jelölje be a **munkafolyamatok**.</span><span class="sxs-lookup"><span data-stu-id="0d37d-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="0d37d-107">A **munkafolyamatok** menüszalag **Új** csoportjában jelölje be **Újrahasználható munkafolyamat**.</span><span class="sxs-lookup"><span data-stu-id="0d37d-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="0d37d-p101">Az **Újrahasználható munkafolyamat létrehozása** űrlapon adja meg a nevét \*\* *Repair2010* \*\*. **Platform típusát**kattintson a **SharePoint 2010 munkafolyamat**, és kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="0d37d-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="0d37d-110">A **munkafolyamat** -menüszalag **mentése** csoportjában jelölje be **a közzététel**.</span><span class="sxs-lookup"><span data-stu-id="0d37d-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="0d37d-p102">A **munkafolyamat** -menüszalag **kezelése** csoportjában válassza **Globálisan közzétenni**. A megjelenő megerősítést kérő párbeszédpanelen kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="0d37d-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="0d37d-p103">Egy webböngészőben keresse meg a legfelső szintű webhely helycsoport, és hozzáférhet a **Webhely beállításai** \> **Webhelycsoport-szolgáltatások**. A **munkafolyamat** -szolgáltatás ezután váltása:</span><span class="sxs-lookup"><span data-stu-id="0d37d-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="0d37d-115">· Ha a szolgáltatás *aktív* , kattintson az **Inaktiválás,** és kattintson az **Aktiválás**.</span><span class="sxs-lookup"><span data-stu-id="0d37d-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="0d37d-116">· Ha a szolgáltatás *inaktívvá válnak* , kattintson az **Aktiválás**.</span><span class="sxs-lookup"><span data-stu-id="0d37d-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="0d37d-117">További információt találhat a következő [cikk](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="0d37d-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

