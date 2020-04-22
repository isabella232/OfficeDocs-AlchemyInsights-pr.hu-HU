---
title: A hiányzó munkafolyamat ot nem sikerült aktiválni
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762103"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="41da7-102">A hiányzó munkafolyamat ot nem sikerült aktiválni</span><span class="sxs-lookup"><span data-stu-id="41da7-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="41da7-103">Microsoft SharePoint-webhelycsoportban nem adhat hozzá globálisan újrafelhasználható munkafolyamatot (például "Jóváhagyás – SharePoint 2010") listához vagy tárhoz.</span><span class="sxs-lookup"><span data-stu-id="41da7-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="41da7-104">A probléma megoldásához hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="41da7-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="41da7-105">Nyissa meg a SharePoint Designer 2013 webhelycsoportgyökérwebhelyét.</span><span class="sxs-lookup"><span data-stu-id="41da7-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="41da7-106">A **Webhelyobjektumok csoportban**válassza a **Munkafolyamatok**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="41da7-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="41da7-107">A **Munkafolyamatok** menüszalag **Új** szakaszában válassza az **Újrafelhasználható munkafolyamat lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="41da7-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="41da7-108">Az **Újrafelhasználható munkafolyamat létrehozása** képernyőn adja meg a \*\* *Repair2010* \*\*nevet.</span><span class="sxs-lookup"><span data-stu-id="41da7-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="41da7-109">A **Platformtípus csoportban**kattintson a **SharePoint 2010-munkafolyamat**elemre, majd az **OK**gombra.</span><span class="sxs-lookup"><span data-stu-id="41da7-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="41da7-110">A **Munkafolyamat** menüszalag **Mentés** szakaszában válassza a **Közzététel**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="41da7-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="41da7-111">A **Munkafolyamat** menüszalag **Kezelés** szakaszában válassza a **Globális közzététel**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="41da7-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="41da7-112">A megjelenő megerősítést kérő párbeszédpanelen válassza az **OK gombot.**</span><span class="sxs-lookup"><span data-stu-id="41da7-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="41da7-113">Keresse meg a webböngészőben a webhelycsoport gyökérwebhelyét, majd érje el a **Webhelybeállítások** \> **webhelycsoport szolgáltatásait.**</span><span class="sxs-lookup"><span data-stu-id="41da7-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="41da7-114">Ezután kapcsolja be a **Munkafolyamatok** funkciót:</span><span class="sxs-lookup"><span data-stu-id="41da7-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="41da7-115">· Ha a szolgáltatás *aktiválva* van, kattintson **az Inaktiválás gombra,** majd az **Aktiválás gombra.**</span><span class="sxs-lookup"><span data-stu-id="41da7-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="41da7-116">· Ha a szolgáltatás *inaktiválva* van, kattintson az **Aktiválás gombra.**</span><span class="sxs-lookup"><span data-stu-id="41da7-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="41da7-117">További információkért kérjük, olvassa el a következő [cikket](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="41da7-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

