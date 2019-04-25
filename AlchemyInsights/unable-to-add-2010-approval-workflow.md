---
title: Nem lehet hozzáadni a jóváhagyási munkafolyamat 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 3741b1169ddf731725c18fbaed80bfb321e5db46
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32366837"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="ebcb2-102">Nem lehet hozzáadni a jóváhagyási munkafolyamat 2010</span><span class="sxs-lookup"><span data-stu-id="ebcb2-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="ebcb2-103">A Microsoft SharePoint-webhelycsoport nem adhat (például a "Jóváhagyás – SharePoint 2010") globálisan újrafelhasználható munkafolyamat listához vagy könyvtárhoz.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="ebcb2-104">A probléma megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="ebcb2-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="ebcb2-105">Nyissa meg a legfelső szintű webhely helycsoport a SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="ebcb2-106">**A helyobjektumok**jelölje be a **munkafolyamatok**.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="ebcb2-107">A **munkafolyamatok** menüszalag **Új** csoportjában jelölje be **Újrahasználható munkafolyamat**.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="ebcb2-108">Az **Újrahasználható munkafolyamat létrehozása** űrlapon adja meg a nevét \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="ebcb2-109">**Platform típusát**kattintson a **SharePoint 2010 munkafolyamat**, és kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="ebcb2-110">A **munkafolyamat** -menüszalag **mentése** csoportjában jelölje be **a közzététel**.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="ebcb2-111">A **munkafolyamat** -menüszalag **kezelése** csoportjában válassza **Globálisan közzétenni**.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="ebcb2-112">A megjelenő megerősítést kérő párbeszédpanelen kattintson az **OK gombra**.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="ebcb2-113">Egy webböngészőben keresse meg a legfelső szintű webhely helycsoport, és hozzáférhet a **Webhely beállításai** \> **Webhelycsoport-szolgáltatások**.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="ebcb2-114">Váltás a **munkafolyamatok** szolgáltatás:</span><span class="sxs-lookup"><span data-stu-id="ebcb2-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="ebcb2-115">· Ha a szolgáltatás *aktív* , kattintson az **Inaktiválás,** és kattintson az **Aktiválás**.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="ebcb2-116">· Ha a szolgáltatás *inaktívvá válnak* , kattintson az **Aktiválás**.</span><span class="sxs-lookup"><span data-stu-id="ebcb2-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="ebcb2-117">További információt találhat a következő [cikk](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="ebcb2-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

