---
title: A Teams élőesemények használatának első lépései
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811962"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="6578a-102">A Teams élőesemények használatának első lépései</span><span class="sxs-lookup"><span data-stu-id="6578a-102">Getting started with Teams live events</span></span>

<span data-ttu-id="6578a-103">A Microsoft Teams élő események a Teams értekezletek kiterjesztése, amely lehetővé teszi az események ütemezését és létrehozását nagyobb online közönségek előtt.</span><span class="sxs-lookup"><span data-stu-id="6578a-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="6578a-104">Élő esemény létrehozásához az alábbiakra lesz szüksége:</span><span class="sxs-lookup"><span data-stu-id="6578a-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="6578a-105">Első lépésként győződjön meg arról, hogy a Teams élő események [elérhetők az Ön országában és régiójában](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); egyes országokban még nem támogatottak az élő események.</span><span class="sxs-lookup"><span data-stu-id="6578a-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="6578a-106">Ha hozzárendelte a licenceket és beállította a házirendeket, de még mindig nem tud Teams élő eseményt létrehozni, akkor valószínűleg olyan országban vagy régióban tartózkodik, ahol még nem érhetők el az élő események.</span><span class="sxs-lookup"><span data-stu-id="6578a-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="6578a-107">Egy [Office 365 nagyvállalati E1, E3 vagy E5 licenc, illetve Office 365 A3 vagy A5 licenc](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="6578a-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="6578a-108">**Megjegyzés**: a Teams használatának közelmúltbeli növekedésének köszönhetően a Teams licencének egy felhasználóhoz rendelését követően a rendszer akár 24 órát is igénybe vehet a teljes beállításhoz.</span><span class="sxs-lookup"><span data-stu-id="6578a-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="6578a-109">Addig is nem fogja tudni a Teams házirendjeit hozzájuk rendelni, és előfordulhat, hogy nem férnek hozzá a Teams néhány funkciójához, például a híváshoz és a hangkonferenciához.</span><span class="sxs-lookup"><span data-stu-id="6578a-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="6578a-110">[Élő események létrehozásának engedélyezése a Microsoft Teams felügyeleti központban](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="6578a-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="6578a-111">[Élő események létrehozásának engedélyezése a Microsoft Streamben](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (külső közvetítési alkalmazással vagy eszközzel létrehozott események esetén).</span><span class="sxs-lookup"><span data-stu-id="6578a-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="6578a-112">Teljes csapatbeli tagság a szervezeten belül (nem lehet vendég vagy egy másik szervezet tagja).</span><span class="sxs-lookup"><span data-stu-id="6578a-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="6578a-113">Személyes értekezletek ütemezése, képernyőmegosztás és IP-videomegosztás bekapcsolása a csapatértekezlet-házirendjében.</span><span class="sxs-lookup"><span data-stu-id="6578a-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="6578a-114">[Ajánlott eljárások](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) Teams élő eseményekhez.</span><span class="sxs-lookup"><span data-stu-id="6578a-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="6578a-115">További információért kérjük, tekintse meg [A Microsoft Teams élő események használatának első lépései](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a) témakört.</span><span class="sxs-lookup"><span data-stu-id="6578a-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>