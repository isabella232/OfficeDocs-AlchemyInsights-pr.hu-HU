---
title: Klasszikus módú SharePoint Online korlátozása
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 6a7c0497243ef7425917f54815e61f1244838c54
ms.sourcegitcommit: b14aa00b42ce4ca9d7dc3aa1fd57e66eae115447
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/28/2019
ms.locfileid: "30953347"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="a3322-102">Klasszikus módú SharePoint Online korlátozása</span><span class="sxs-lookup"><span data-stu-id="a3322-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="a3322-103">Egyes szervezetek továbbra is csak a klasszikus mód tapasztalat.</span><span class="sxs-lookup"><span data-stu-id="a3322-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="a3322-104">Nem is tervezzük alapszinten Klasszikus módú eltávolítása, míg indítása április 1,2019, hogy többé nem lehet korlátozni a teljes szervezet (bérlő) listák és tárak klasszikus módba.</span><span class="sxs-lookup"><span data-stu-id="a3322-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="a3322-105">Az admin lesz egyéni listák és tárak klasszikus módban kapcsolókkal granulált lemondja, amit adunk a következő szinteken kezelheti a következők:</span><span class="sxs-lookup"><span data-stu-id="a3322-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

<span data-ttu-id="a3322-106">----webhely--webhelycsoportok listája--könyvtár</span><span class="sxs-lookup"><span data-stu-id="a3322-106">-- site collection -- site -- list -- library</span></span>

<span data-ttu-id="a3322-107">Ezenkívül bizonyos szolgáltatásokat használó listák és modern által nem támogatott testreszabási beállításokat fogja továbbra is lehet automatikusan üzemmódba kell kapcsolni klasszikus.</span><span class="sxs-lookup"><span data-stu-id="a3322-107">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="a3322-108">Után április 1 listák és tárak, amelyek eredményeként a bérlő opt-out klasszikus módban automatikusan kezelik a webhely szinten és a szint.</span><span class="sxs-lookup"><span data-stu-id="a3322-108">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="a3322-109">Klasszikus módú van szüksége további információt itt talál, és a PnP Powershell utasítás itt, amely leírja a beállítások és eszközök segítségével ma előkészítése a helyi szintű lemondja április 1-jén megszüntetését.</span><span class="sxs-lookup"><span data-stu-id="a3322-109">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
