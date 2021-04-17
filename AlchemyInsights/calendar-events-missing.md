---
title: Hiányoznak vagy nem frissülnek a naptáresemények
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837390"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="819de-102">Hiányoznak vagy nem frissülnek a naptáresemények</span><span class="sxs-lookup"><span data-stu-id="819de-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="819de-103">Ha hiányoznak vagy nem frissülnek a naptárelemek, először is az Outlook Naptár mappájának tulajdonságaiban lévő elemek számát kell keresnie:</span><span class="sxs-lookup"><span data-stu-id="819de-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="819de-104">Kattintson a jobb gombbal az érintett felhasználói **naptár mappára,** és válassza a Tulajdonságok **parancsot.**</span><span class="sxs-lookup"><span data-stu-id="819de-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="819de-105">Válassza a **Szinkronizálás fület.**</span><span class="sxs-lookup"><span data-stu-id="819de-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="819de-106">Ha az elemszám nem azonos a Kiszolgáló és a Kapcsolat nélküli mappa között:</span><span class="sxs-lookup"><span data-stu-id="819de-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="819de-107">Jelölje ki **a Naptár** mappát.</span><span class="sxs-lookup"><span data-stu-id="819de-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="819de-108">A Küldés  / **fogadása lapon** válassza a Mappa frissítése **lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="819de-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="819de-109">Ha a naptára még mindig nem frissül, vagy ha hiányoznak az események, töltse le az Outlook naptárellenőri eszközét a [Microsoft letöltőközpontból.](https://www.microsoft.com/download/details.aspx?id=28786)</span><span class="sxs-lookup"><span data-stu-id="819de-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="819de-110">Állapítsa meg, hogy több mint 5000 elem található-e a naptármappában, mivel ez olyan jelenségeket okozhat, mint például a nem frissülő naptári értekezletek vagy értekezlethibák.</span><span class="sxs-lookup"><span data-stu-id="819de-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="819de-111">További információ: Az Outlook teljesítményével kapcsolatos problémák, ha túl sok elem vagy mappa van gyorsítótáras üzemmódban [.ost vagy .pst fájlban.](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)</span><span class="sxs-lookup"><span data-stu-id="819de-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>