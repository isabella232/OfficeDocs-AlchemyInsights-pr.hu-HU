---
title: A diagram különböző számú rekordot jelenít meg a rácsban
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439354"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="5d61f-102">A diagram különböző számú rekordot jelenít meg a rácsban</span><span class="sxs-lookup"><span data-stu-id="5d61f-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="5d61f-103">**Tünet**</span><span class="sxs-lookup"><span data-stu-id="5d61f-103">**Symptom**</span></span>

<span data-ttu-id="5d61f-104">A diagram műszerfal oldalon, ha rákattint a diagram "..." és kattintson a "Rekordok megtekintése", akkor keresse meg a rács oldalon, hogy az összes rekordot. Néha megváltozik a rekordok száma.</span><span class="sxs-lookup"><span data-stu-id="5d61f-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="5d61f-105">**A probléma oka**</span><span class="sxs-lookup"><span data-stu-id="5d61f-105">**Cause**</span></span>

<span data-ttu-id="5d61f-106">Ennek oka az eredeti irányítópult-oldalon lévő diagram és a rács kezdőlapján lévő diagram közötti nézetkülönbség.</span><span class="sxs-lookup"><span data-stu-id="5d61f-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="5d61f-107">**Megoldás**</span><span class="sxs-lookup"><span data-stu-id="5d61f-107">**Solution**</span></span>

1. <span data-ttu-id="5d61f-108">Ellenőrizze az eredeti oldal nézetét és a rács nézetét, és ellenőrizze, hogy különböznek-e.</span><span class="sxs-lookup"><span data-stu-id="5d61f-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="5d61f-109">Módosítsa a rács nézetét úgy, hogy az megfeleljen az eredeti oldal nézetének.</span><span class="sxs-lookup"><span data-stu-id="5d61f-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="5d61f-110">Ha a megfelelő nézet nem található, az általában azt jelenti, hogy a nézet nincs engedélyezve az alkalmazástervezőben.</span><span class="sxs-lookup"><span data-stu-id="5d61f-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="5d61f-111">Nyissa meg az adott alkalmazás alkalmazástervezőjét, válassza ki az entitást és annak nézeteit, ellenőrizze az engedélyezni, menteni, közzétenni és bezárni kívánt nézetet.</span><span class="sxs-lookup"><span data-stu-id="5d61f-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="5d61f-112">Frissítse a lapot.</span><span class="sxs-lookup"><span data-stu-id="5d61f-112">Refresh the page.</span></span>