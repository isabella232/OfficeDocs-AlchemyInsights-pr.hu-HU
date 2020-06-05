---
title: Nem lehet hozzáadni a 2010-es jóváhagyási munkafolyamatot
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582849"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="61106-102">Nem lehet hozzáadni a 2010-es jóváhagyási munkafolyamatot</span><span class="sxs-lookup"><span data-stu-id="61106-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="61106-103">Microsoft SharePoint-webhelycsoportban nem adhat hozzá globálisan újrafelhasználható munkafolyamatot (például "Jóváhagyás – SharePoint 2010") listához vagy tárhoz.</span><span class="sxs-lookup"><span data-stu-id="61106-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="61106-104">A probléma megoldásához hajtsa végre az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="61106-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="61106-105">Nyissa meg a SharePoint Designer 2013 webhelycsoportgyökérwebhelyét.</span><span class="sxs-lookup"><span data-stu-id="61106-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="61106-106">A **Webhelyobjektumok csoportban**válassza a **Munkafolyamatok**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="61106-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="61106-107">A **Munkafolyamatok** menüszalag **Új** szakaszában válassza az **Újrafelhasználható munkafolyamat lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="61106-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="61106-108">Az **Újrafelhasználható munkafolyamat létrehozása** képernyőn adja meg a \*\* *Repair2010* \*\*nevet.</span><span class="sxs-lookup"><span data-stu-id="61106-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="61106-109">A **Platformtípus csoportban**kattintson a **SharePoint 2010-munkafolyamat**elemre, majd az **OK**gombra.</span><span class="sxs-lookup"><span data-stu-id="61106-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="61106-110">A **Munkafolyamat** menüszalag **Mentés** szakaszában válassza a **Közzététel**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="61106-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="61106-111">A **Munkafolyamat** menüszalag **Kezelés** szakaszában válassza a **Globális közzététel**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="61106-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="61106-112">A megjelenő megerősítést kérő párbeszédpanelen válassza az **OK gombot.**</span><span class="sxs-lookup"><span data-stu-id="61106-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="61106-113">Keresse meg a webböngészőben a webhelycsoport gyökérwebhelyét, majd érje el a **Webhelybeállítások** \> **webhelycsoport szolgáltatásait.**</span><span class="sxs-lookup"><span data-stu-id="61106-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="61106-114">A Munkafolyamatok szolgáltatás **bekapcsolása:**</span><span class="sxs-lookup"><span data-stu-id="61106-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="61106-115">· Ha a szolgáltatás *aktiválva* van, kattintson **az Inaktiválás gombra,** majd az **Aktiválás gombra.**</span><span class="sxs-lookup"><span data-stu-id="61106-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="61106-116">· Ha a szolgáltatás *inaktiválva* van, kattintson az **Aktiválás gombra.**</span><span class="sxs-lookup"><span data-stu-id="61106-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="61106-117">További információkért kérjük, olvassa el a következő [cikket](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="61106-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

