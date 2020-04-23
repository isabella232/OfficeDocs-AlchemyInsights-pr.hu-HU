---
title: Nagy SharePoint-listák
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767287"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="c4949-102">Nagylisták és tárak használata a SharePointban</span><span class="sxs-lookup"><span data-stu-id="c4949-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="c4949-103">A SharePoint-listák és -tárak legfeljebb 30 millió elemet tartalmazhatnak, de ha több mint 5000 elem ből állnak, előfordulhat, hogy a listanézet küszöbértéke hibaüzenet jelenik meg, amikor dolgozni próbál velük.</span><span class="sxs-lookup"><span data-stu-id="c4949-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="c4949-104">A küszöbértéket a szolgáltatás ideális teljesítményének fenntartása érdekében állítottuk be.</span><span class="sxs-lookup"><span data-stu-id="c4949-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="c4949-105">A felhasználók ezt nem módosíthatják.</span><span class="sxs-lookup"><span data-stu-id="c4949-105">It can't be changed.</span></span> <span data-ttu-id="c4949-106">Annak elkerülése érdekében, hogy eltalálja ezt a küszöbértéket:</span><span class="sxs-lookup"><span data-stu-id="c4949-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="c4949-107">**Modern használata**</span><span class="sxs-lookup"><span data-stu-id="c4949-107">**Use modern**</span></span>

<span data-ttu-id="c4949-108">A sok elemet megjelenítő nézetek a modern élményben működnek a legjobban.</span><span class="sxs-lookup"><span data-stu-id="c4949-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="c4949-109">[Használja a modern élményt,](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) hogy elkerülje a klasszikus élményben látható hibákat.</span><span class="sxs-lookup"><span data-stu-id="c4949-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="c4949-110">**Indexek hozzáadása**</span><span class="sxs-lookup"><span data-stu-id="c4949-110">**Add indexes**</span></span>

<span data-ttu-id="c4949-111">Ha olyan oszlop ot szűr vagy rendez, amely nem rendelkezik indexszel, hibaüzenet jelenhet meg.</span><span class="sxs-lookup"><span data-stu-id="c4949-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="c4949-112">[A](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) Beállítások menü **Listabeállítások menüjének listaelem-listájának** manuális hozzáadása az **Indexet**.</span><span class="sxs-lookup"><span data-stu-id="c4949-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="c4949-113">**A listanézet szerkesztése**</span><span class="sxs-lookup"><span data-stu-id="c4949-113">**Edit the list view**</span></span>

<span data-ttu-id="c4949-114">Ha nagy lista esetén hiba történik, [szerkesztsd a listanézetet.](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)</span><span class="sxs-lookup"><span data-stu-id="c4949-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="c4949-115">A következő négy módosítás eltávolítja a listanézet küszöbértékhibáit.</span><span class="sxs-lookup"><span data-stu-id="c4949-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="c4949-116">Az összes hiba eltávolításához hajtsa végre mind a négy módosítást.</span><span class="sxs-lookup"><span data-stu-id="c4949-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="c4949-117">Ha továbbra is hibákat tapasztal, jelölje be [A nagyméretű listák és tárak kezelése jelölőnégyzetet.](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)</span><span class="sxs-lookup"><span data-stu-id="c4949-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="c4949-118">Válassza a **Nincs** elemet az **Első rendezés oszlop szerint,** majd az oszlop szerint rendezés **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="c4949-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="c4949-119">Válassza a **Nincs** lehetőséget az **első csoportból az oszlop szerint,** **majd az oszlop szerint csoportosítva**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c4949-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="c4949-120">Válassza a **Nincs** lehetőséget az **Összesítés** szakasz összes oszlopára.</span><span class="sxs-lookup"><span data-stu-id="c4949-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="c4949-121">Törölje az összes, egy kivételével látható oszlop ot az **Oszlopok** szakaszból.</span><span class="sxs-lookup"><span data-stu-id="c4949-121">Deselect all but one column for display from the **Columns** section.</span></span>

