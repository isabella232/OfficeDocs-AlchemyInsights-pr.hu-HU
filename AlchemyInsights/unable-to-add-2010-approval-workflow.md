---
title: Nem lehet felvenni a 2010-jóváhagyási munkafolyamatot
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699737"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="3606c-102">Nem lehet felvenni a 2010-jóváhagyási munkafolyamatot</span><span class="sxs-lookup"><span data-stu-id="3606c-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="3606c-103">A Microsoft SharePoint-webhelycsoportban nem lehet globálisan újrafelhasználható munkafolyamatot (például "jóváhagyás – SharePoint 2010") hozzáadni egy listához vagy tárhoz.</span><span class="sxs-lookup"><span data-stu-id="3606c-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="3606c-104">A probléma megoldásához kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="3606c-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="3606c-105">Nyissa meg a webhelycsoport legfelső szintű webhelyét a SharePoint Designer 2013-ban.</span><span class="sxs-lookup"><span data-stu-id="3606c-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="3606c-106">A **hely objektumai**csoportban válassza a **munkafolyamatok**elemet.</span><span class="sxs-lookup"><span data-stu-id="3606c-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="3606c-107">A **munkafolyamatok** menüszalagjának **új** szakaszában válassza az **újból felhasználható munkafolyamat**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3606c-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="3606c-108">Az **újrafelhasználható munkafolyamat létrehozása** űrlapon írja be a \* \* *Repair2010* \* \* nevet.</span><span class="sxs-lookup"><span data-stu-id="3606c-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="3606c-109">**Platform típusa**esetén kattintson a **SharePoint 2010 munkafolyamat**elemre, majd kattintson **az OK**gombra.</span><span class="sxs-lookup"><span data-stu-id="3606c-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="3606c-110">A **munkafolyamat** menüszalagjának **Mentés** szakaszában válassza a **Közzététel**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3606c-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="3606c-111">A **munkafolyamat** menüszalagjának **Manage (kezelés** ) szakaszában válassza a **globális közzététel**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="3606c-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="3606c-112">A megjelenő megerősítést kérő párbeszédpanelen válassza az **OK gombot**.</span><span class="sxs-lookup"><span data-stu-id="3606c-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="3606c-113">A webböngészőben keresse meg a webhelycsoport legfelső szintű webhelyét, és nyissa meg a webhely **beállításai** – webhelycsoport \> **funkcióit**.</span><span class="sxs-lookup"><span data-stu-id="3606c-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="3606c-114">A **munkafolyamatok** funkció bekapcsolása:</span><span class="sxs-lookup"><span data-stu-id="3606c-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="3606c-115">· Ha a funkció  *aktiválva*  van, kattintson az **Inaktiválás gombra,** majd az **aktiválás**parancsra.</span><span class="sxs-lookup"><span data-stu-id="3606c-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="3606c-116">· Ha a funkció  *inaktiválva*  van, kattintson az **aktiválás**gombra.</span><span class="sxs-lookup"><span data-stu-id="3606c-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="3606c-117">További információért olvassa el a következő [cikket](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="3606c-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

