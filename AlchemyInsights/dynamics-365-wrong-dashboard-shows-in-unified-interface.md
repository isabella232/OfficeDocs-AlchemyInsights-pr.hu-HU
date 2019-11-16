---
title: Dynamics 365-hibás irányítópult-műsorok Dynamics 365 egyesített illesztő
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528553"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="f8243-102">Hibás irányítópult-bemutatók a Dynamics 365 egységes illesztőfelületen</span><span class="sxs-lookup"><span data-stu-id="f8243-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="f8243-103">Több oka is lehet, hogy miért jelenik meg egy másik irányítópult, mint amit elvársz:</span><span class="sxs-lookup"><span data-stu-id="f8243-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="f8243-104">A felhasználó beállította a felhasználó alapértelmezett irányítópultját</span><span class="sxs-lookup"><span data-stu-id="f8243-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="f8243-105">Általában akkor lehet azonosítani egy felhasználói alapértelmezett irányítópultot, ha az **alapértelmezés szerinti beállítás** gomb nem jelenik meg az irányítópult parancssávján.</span><span class="sxs-lookup"><span data-stu-id="f8243-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="f8243-106">A felhasználó alapértelmezett irányítópultja felülírja az összes többi alapértelmezett irányítópultot még akkor is, ha a felhasználó alapértelmezett irányítópultja nem szerepel az aktuális alkalmazásban.</span><span class="sxs-lookup"><span data-stu-id="f8243-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="f8243-107">A következő kerülő megoldás segítségével állítsa be az alapértelmezett irányítópultot.</span><span class="sxs-lookup"><span data-stu-id="f8243-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="f8243-108">Hozzon létre egy új személyes irányítópultot.</span><span class="sxs-lookup"><span data-stu-id="f8243-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="f8243-109">Az új irányítópult beállítása felhasználói alapértelmezésként.</span><span class="sxs-lookup"><span data-stu-id="f8243-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="f8243-110">Törölje az irányítópultot.</span><span class="sxs-lookup"><span data-stu-id="f8243-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="f8243-111">A műszerfal van készlet-ban sitemap</span><span class="sxs-lookup"><span data-stu-id="f8243-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="f8243-112">Lehet, hogy beállította a szervezet alapértelmezett irányítópultját az irányítópult kijelölésével és a "beállítás alapértelmezettként" választásával a "rendszer testreszabása" címszó alatt.</span><span class="sxs-lookup"><span data-stu-id="f8243-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="f8243-113">A webhelytérkép-tervezőben definiált irányítópult azonban elsőbbséget élvez az irányítópulttal szemben, ha a felhasználónak hozzáférése van hozzá.</span><span class="sxs-lookup"><span data-stu-id="f8243-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="f8243-114">Ha azt szeretné, hogy a felhasználók a szervezet alapértelmezettnek tekintse meg az irányítópultot, az alábbiak közül választhat:</span><span class="sxs-lookup"><span data-stu-id="f8243-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="f8243-115">Az irányítópult beállítása a webhelytérképben</span><span class="sxs-lookup"><span data-stu-id="f8243-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="f8243-116">Távolítsa el a hozzáférést a webhelytérkép definiált irányítópulthoz a felhasználók számára</span><span class="sxs-lookup"><span data-stu-id="f8243-116">Remove access to the sitemap defined dashboard for those users</span></span>
