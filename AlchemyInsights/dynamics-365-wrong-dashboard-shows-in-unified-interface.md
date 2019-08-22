---
title: Dynamics 365 - rossz irányítópult Dynamics 365 egységes felületen látható
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528553"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="f444a-102">Rossz irányítópult Dynamics 365 egységes felületen jeleníti meg</span><span class="sxs-lookup"><span data-stu-id="f444a-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="f444a-103">Több oka miért várt egy másik irányítópult jelenhetnek meg:</span><span class="sxs-lookup"><span data-stu-id="f444a-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="f444a-104">A felhasználó be van állítva az alapértelmezett felhasználói irányítópult</span><span class="sxs-lookup"><span data-stu-id="f444a-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="f444a-105">Általában azonosítani tudja a felhasználót ha az **Alapértelmezett** gomb nem jelenik meg a parancssávon irányítópult beállítása alapértelmezett irányítópultot.</span><span class="sxs-lookup"><span data-stu-id="f444a-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="f444a-106">Az alapértelmezett felhasználói irányítópult felülírják más alapértelmezett irányítópultok, még akkor is, ha az aktuális alkalmazás nem szerepel a felhasználó alapértelmezett irányítópultot.</span><span class="sxs-lookup"><span data-stu-id="f444a-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="f444a-107">Használja az alábbi megoldásokat az Adatbázisjelszó törlése az alapértelmezett irányítópultot.</span><span class="sxs-lookup"><span data-stu-id="f444a-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="f444a-108">Hozzon létre egy új személyes irányítópult.</span><span class="sxs-lookup"><span data-stu-id="f444a-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="f444a-109">Ez új irányítópult beállítása a felhasználó alapértelmezett.</span><span class="sxs-lookup"><span data-stu-id="f444a-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="f444a-110">Adott irányítópult törlése.</span><span class="sxs-lookup"><span data-stu-id="f444a-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="f444a-111">Az irányítópult van megadva az Oldaltérkép</span><span class="sxs-lookup"><span data-stu-id="f444a-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="f444a-112">Beállított egy szervezet alapértelmezett irányítópultot irányítópult kijelölésével, majd válassza a "Alapértelmezett" "A rendszer testreszabása" alatt.</span><span class="sxs-lookup"><span data-stu-id="f444a-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="f444a-113">De az irányítópult a webhelytérkép-tervezőben meghatározott elsőbbséget élveznek az irányítópultot, ha a felhasználónak van hozzáférése.</span><span class="sxs-lookup"><span data-stu-id="f444a-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="f444a-114">Ahhoz, hogy a felhasználók megtekinthetik a szervezet alapértelmezett beállítása az irányítópultot, közül választhat:</span><span class="sxs-lookup"><span data-stu-id="f444a-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="f444a-115">Az oldaltérkép az adott irányítópult beállítása</span><span class="sxs-lookup"><span data-stu-id="f444a-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="f444a-116">Távolítsa el a felhasználók hozzáférését az Oldaltérkép definiált irányítópulton</span><span class="sxs-lookup"><span data-stu-id="f444a-116">Remove access to the sitemap defined dashboard for those users</span></span>
