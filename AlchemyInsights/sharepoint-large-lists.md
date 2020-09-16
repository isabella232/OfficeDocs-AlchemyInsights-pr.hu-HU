---
title: Nagyméretű SharePoint-listák
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720135"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="1ded8-102">Nagyméretű listák és tárak használata a SharePointban</span><span class="sxs-lookup"><span data-stu-id="1ded8-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="1ded8-103">A SharePoint-listák és-tárak 30 000 000-elemeket tartalmazhatnak, de ha több mint 5 000-elemük van, előfordulhat, hogy a lista nézet küszöbértéke hibaüzenet jelenik meg, amikor megpróbál dolgozni velük.</span><span class="sxs-lookup"><span data-stu-id="1ded8-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="1ded8-104">A küszöbértéket a szolgáltatás ideális teljesítményének fenntartása érdekében állítottuk be.</span><span class="sxs-lookup"><span data-stu-id="1ded8-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="1ded8-105">A felhasználók ezt nem módosíthatják.</span><span class="sxs-lookup"><span data-stu-id="1ded8-105">It can't be changed.</span></span> <span data-ttu-id="1ded8-106">Ha el szeretné kerülni, hogy ne verjék ezt a küszöböt:</span><span class="sxs-lookup"><span data-stu-id="1ded8-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="1ded8-107">**A modern használata**</span><span class="sxs-lookup"><span data-stu-id="1ded8-107">**Use modern**</span></span>

<span data-ttu-id="1ded8-108">A sok elemet megjelenítő nézetek a modern felületeken működnek a legjobban.</span><span class="sxs-lookup"><span data-stu-id="1ded8-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="1ded8-109">[A modern felülettel](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) elkerülhetők a klasszikus élményben esetlegesen megjelenő hibák.</span><span class="sxs-lookup"><span data-stu-id="1ded8-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="1ded8-110">**Indexek hozzáadása**</span><span class="sxs-lookup"><span data-stu-id="1ded8-110">**Add indexes**</span></span>

<span data-ttu-id="1ded8-111">Ha olyan oszlopot szűr vagy rendez, amelynek nincs indexe, hibaüzenetet kaphat.</span><span class="sxs-lookup"><span data-stu-id="1ded8-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="1ded8-112">A beállítások menüben, majd az **indexelt oszlopokban**a **lista beállításai** között manuálisan [vehet fel indexet](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) .</span><span class="sxs-lookup"><span data-stu-id="1ded8-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="1ded8-113">**A lista nézet szerkesztése**</span><span class="sxs-lookup"><span data-stu-id="1ded8-113">**Edit the list view**</span></span>

<span data-ttu-id="1ded8-114">Ha egy nagyméretű lista használatakor hiba történik, [szerkessze a lista nézetét](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="1ded8-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="1ded8-115">A következő négy módosítás eltávolítja a lista nézet küszöbének hibáit.</span><span class="sxs-lookup"><span data-stu-id="1ded8-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="1ded8-116">Az összes hiba eltávolításához végezze el mind a négy módosítást.</span><span class="sxs-lookup"><span data-stu-id="1ded8-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="1ded8-117">Ha továbbra is hibát tapasztal, jelölje be a [nagyméretű listák és tárak kezelése](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="1ded8-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="1ded8-118">Válassza a **nincs** lehetőséget a mind az **első Rendezés** , mind az oszlop szerinti **Rendezés**lehetőséget választva.</span><span class="sxs-lookup"><span data-stu-id="1ded8-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="1ded8-119">Válassza a **nincs** lehetőséget **az első csoporttól az oszlopnál** , **majd a csoportosítás az oszlop alapján**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1ded8-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="1ded8-120">Válassza a **nincs** lehetőséget az összes oszlop esetében az **Összesítés** szakaszban.</span><span class="sxs-lookup"><span data-stu-id="1ded8-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="1ded8-121">Törölje az összes, de egy oszlop kijelölését az **oszlopok** szakaszból.</span><span class="sxs-lookup"><span data-stu-id="1ded8-121">Deselect all but one column for display from the **Columns** section.</span></span>

