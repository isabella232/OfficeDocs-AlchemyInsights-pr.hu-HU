---
title: A Dynamics 365-a Dynamics 365-ban az egyesített felületen nem jelenik meg a megfelelő irányítópult
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711277"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="c2571-102">Helytelen irányítópult-bemutató a Dynamics 365 egyesített felületén</span><span class="sxs-lookup"><span data-stu-id="c2571-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="c2571-103">Több oka lehet annak, ha a várttól eltérő irányítópult jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="c2571-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="c2571-104">A felhasználó beállított egy felhasználó alapértelmezett irányítópultot</span><span class="sxs-lookup"><span data-stu-id="c2571-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="c2571-105">Általában akkor lehet megállapítani, ha a felhasználó alapértelmezett irányítópultja van beállítva, ha a **Beállítás alapértelmezettként** gomb nem jelenik meg az irányítópult-parancssorban.</span><span class="sxs-lookup"><span data-stu-id="c2571-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="c2571-106">A felhasználó alapértelmezett irányítópultja felülírja az összes többi alapértelmezett irányítópultot, még akkor is, ha a felhasználó alapértelmezett irányítópultja nem szerepel az aktuális alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="c2571-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="c2571-107">Az alapértelmezett irányítópult törléséhez használja az alábbi kerülő megoldást.</span><span class="sxs-lookup"><span data-stu-id="c2571-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="c2571-108">Hozzon létre egy új személyes irányítópultot.</span><span class="sxs-lookup"><span data-stu-id="c2571-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="c2571-109">Állítsa be az új irányítópultot alapértelmezettként.</span><span class="sxs-lookup"><span data-stu-id="c2571-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="c2571-110">Törölje az irányítópultot.</span><span class="sxs-lookup"><span data-stu-id="c2571-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="c2571-111">Az irányítópult a webhelytérképben van beállítva</span><span class="sxs-lookup"><span data-stu-id="c2571-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="c2571-112">Lehet, hogy a szervezet alapértelmezett irányítópultját egy irányítópult kijelölésével, majd a "rendszer testreszabása" elemre kattintva választhatja ki.</span><span class="sxs-lookup"><span data-stu-id="c2571-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="c2571-113">A webhelytérkép-tervezőben definiált irányítópult azonban előnyben részesíti az irányítópultot, ha a felhasználó hozzáféréssel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="c2571-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="c2571-114">Ha azt szeretné, hogy a felhasználók a szervezeti alapértelmezettként beállított irányítópultot lássák, az alábbiakat teheti:</span><span class="sxs-lookup"><span data-stu-id="c2571-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="c2571-115">Az irányítópult beállítása a webhelytérképben</span><span class="sxs-lookup"><span data-stu-id="c2571-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="c2571-116">A webhelytérképhez meghatározott irányítópult elérésének megszüntetése a felhasználóknak</span><span class="sxs-lookup"><span data-stu-id="c2571-116">Remove access to the sitemap defined dashboard for those users</span></span>
