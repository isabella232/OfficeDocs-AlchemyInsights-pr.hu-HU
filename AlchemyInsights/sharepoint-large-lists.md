---
title: SharePoint-nagyméretű listák
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488519"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="4cfe5-102">Nagyméretű listák és tárak munka SharePoint rendszerben</span><span class="sxs-lookup"><span data-stu-id="4cfe5-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="4cfe5-103">A SharePoint-listák és-tárak akár 30 000 000 elemeket is tartalmazhatnak, de amikor több mint 5 000 elemet tartalmaznak, a listanézet küszöbe hibaüzenetet láthatja, amikor megpróbál dolgozni velük.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="4cfe5-104">Ez a küszöbérték a szolgáltatás teljesítésének fenntartásához van érvényben.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="4cfe5-105">Nem lehet megváltoztatni.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-105">It can't be changed.</span></span> <span data-ttu-id="4cfe5-106">Hogy elkerüljék üti ezt a küszöböt:</span><span class="sxs-lookup"><span data-stu-id="4cfe5-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="4cfe5-107">**Használja a modern**</span><span class="sxs-lookup"><span data-stu-id="4cfe5-107">**Use modern**</span></span>

<span data-ttu-id="4cfe5-108">A sok elemet bemutató nézetek a legmegfelelőebben működnek a modern élményben.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="4cfe5-109">[Használja a modern élményt](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) a klasszikus élményben esetleg előforduló hibák elkerüléséhez.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="4cfe5-110">**Indexek hozzáadása**</span><span class="sxs-lookup"><span data-stu-id="4cfe5-110">**Add indexes**</span></span>

<span data-ttu-id="4cfe5-111">Ha indexszel nem rendelkező oszlop szerint szűrnek vagy rendeznek, hibaüzenet jelenhet meg.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="4cfe5-112">[Adjon hozzá egy indexet](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) kézzel a **lista beállításaitól** a beállítások menüben, majd az **indexelt oszlopokban**.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="4cfe5-113">**Listanézet szerkesztése**</span><span class="sxs-lookup"><span data-stu-id="4cfe5-113">**Edit the list view**</span></span>

<span data-ttu-id="4cfe5-114">Ha egy nagyméretű listával végzett munka során hiba lép fel, [szerkessze a listanézet](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="4cfe5-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="4cfe5-115">A következő négy módosítás eltávolítja a listanézet küszöbhibáit.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="4cfe5-116">Mind a négy változtatás, hogy távolítsa el az összes hibát.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="4cfe5-117">Ha továbbra is hibákba kezd, ellenőrizze a [nagyméretű listák és tárak kezelését](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="4cfe5-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="4cfe5-118">**Az első rendezéshez** válassza a **nincs** lehetőséget, **majd az oszlop szerint rendezze őket**.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="4cfe5-119">Jelölje ki az első csoport **egyik sem** **csoportját az oszlop szerint** , majd **csoportosítse az oszlop szerint**.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="4cfe5-120">Az **összesítőrész** összes oszlopán válassza a **nincs** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="4cfe5-121">Az **oszlopok** szakaszban megjelenítendő összes, de egy oszlopot törölnek.</span><span class="sxs-lookup"><span data-stu-id="4cfe5-121">Deselect all but one column for display from the **Columns** section.</span></span>

