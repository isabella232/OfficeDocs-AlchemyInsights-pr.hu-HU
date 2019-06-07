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
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761761"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="dec1c-102">Klasszikus módú SharePoint Online korlátozása</span><span class="sxs-lookup"><span data-stu-id="dec1c-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="dec1c-103">Egyes szervezetek továbbra is csak a klasszikus mód tapasztalat.</span><span class="sxs-lookup"><span data-stu-id="dec1c-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="dec1c-104">Nem tervezik alapszinten Klasszikus módú eltávolítása, amíg már nem korlátozhatja a klasszikus módban a listák és tárak teljes szervezeten (bérlő) lehetséges.</span><span class="sxs-lookup"><span data-stu-id="dec1c-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="dec1c-105">Az admin lesz egyéni listák és tárak klasszikus módban kapcsolókkal granulált lemondja, amit adunk a következő szinteken kezelheti a következők:</span><span class="sxs-lookup"><span data-stu-id="dec1c-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="dec1c-106">webhelycsoport</span><span class="sxs-lookup"><span data-stu-id="dec1c-106">site collection</span></span>
- <span data-ttu-id="dec1c-107">webhely</span><span class="sxs-lookup"><span data-stu-id="dec1c-107">site</span></span>
- <span data-ttu-id="dec1c-108">lista</span><span class="sxs-lookup"><span data-stu-id="dec1c-108">list</span></span>
- <span data-ttu-id="dec1c-109">dokumentumtár</span><span class="sxs-lookup"><span data-stu-id="dec1c-109">library</span></span>

<span data-ttu-id="dec1c-110">Ezenkívül bizonyos szolgáltatásokat használó listák és modern által nem támogatott testreszabási beállításokat fogja továbbra is lehet automatikusan üzemmódba kell kapcsolni klasszikus.</span><span class="sxs-lookup"><span data-stu-id="dec1c-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="dec1c-111">Kezdődő április 1, 2019, a folyamat letiltása a bérlő szint befejezése mellett modern lista és könyvtárak elindítja, és folytassa a 2019 május 31-ig.</span><span class="sxs-lookup"><span data-stu-id="dec1c-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="dec1c-112">A listák és tárak, amelyek eredményeként a bérlő opt-out klasszikus módban a program automatikusan kell mozgatni, hogy a modern.</span><span class="sxs-lookup"><span data-stu-id="dec1c-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="dec1c-113">Ha a klasszikus módban van szüksége további információt talál [Itt](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) és a PnP Powershell instruction [Itt](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , amely leírja a beállítások és eszközök segítségével ma a klasszikus módban felület használatára.</span><span class="sxs-lookup"><span data-stu-id="dec1c-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
