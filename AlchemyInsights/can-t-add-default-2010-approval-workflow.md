---
title: Nem lehet hozzáadni az alapértelmezett jóváhagyási munkafolyamat 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293068"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="0f4e6-102">Nem lehet hozzáadni az alapértelmezett jóváhagyási munkafolyamat 2010</span><span class="sxs-lookup"><span data-stu-id="0f4e6-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="0f4e6-103">A Microsoft SharePoint-webhelycsoport nem adhat (például a "Jóváhagyás – SharePoint 2010") globálisan újrafelhasználható munkafolyamat listához vagy könyvtárhoz.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="0f4e6-104">A probléma megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="0f4e6-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="0f4e6-105">Nyissa meg a legfelső szintű webhely helycsoport a SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="0f4e6-106">**A helyobjektumok**jelölje be a **munkafolyamatok**.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="0f4e6-107">A **munkafolyamatok** menüszalag **Új** csoportjában jelölje be **Újrahasználható munkafolyamat**.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="0f4e6-p101">Az **Újrahasználható munkafolyamat létrehozása** űrlapon adja meg nevét \* \*\*Repair2010\*\*\*. **Platform típusa**jelölje be a **SharePoint 2010 munkafolyamat**, és kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="0f4e6-110">A **munkafolyamat** -menüszalag **mentése** csoportjában jelölje be **a közzététel**.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="0f4e6-p102">A **munkafolyamat** -menüszalag **kezelése** csoportjában válassza **Globálisan közzétenni**. A megjelenő megerősítést kérő párbeszédpanelen kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="0f4e6-p103">Egy webböngészőben keresse meg a legfelső szintű webhely helycsoport, és hozzáférhet a **Webhely beállításai** \> **Webhelycsoport-szolgáltatások**. A **munkafolyamat** -szolgáltatás ezután váltása:</span><span class="sxs-lookup"><span data-stu-id="0f4e6-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="0f4e6-115">· Ha a szolgáltatás *aktív* , kattintson az **Inaktiválás,** és kattintson az **Aktiválás**.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="0f4e6-116">· Ha a szolgáltatás *inaktívvá válnak* , kattintson az **Aktiválás**.</span><span class="sxs-lookup"><span data-stu-id="0f4e6-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="0f4e6-117">További információt találhat a következő [cikk](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="0f4e6-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

