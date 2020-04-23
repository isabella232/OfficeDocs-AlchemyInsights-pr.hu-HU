---
title: A SharePoint Online klasszikus módra korlátozása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742471"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="64c5a-102">A SharePoint Online klasszikus módra korlátozása</span><span class="sxs-lookup"><span data-stu-id="64c5a-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="64c5a-103">Egyes szervezetektovábbra is megkövetelik a klasszikus mód élményt.</span><span class="sxs-lookup"><span data-stu-id="64c5a-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="64c5a-104">Bár nem tervezi, hogy távolítsa el a klasszikus mód egy részletes szinten, már nem lehet korlátozni a teljes szervezet (bérlő) a klasszikus mód listák és tárak.</span><span class="sxs-lookup"><span data-stu-id="64c5a-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="64c5a-105">A rendszergazda a következő lehetőségekkel kezeli az egyes listákat és könyvtárakat klasszikus módban a következő szinteken biztosított részletes leiratkozási kapcsolókkal:</span><span class="sxs-lookup"><span data-stu-id="64c5a-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="64c5a-106">webhelycsoport</span><span class="sxs-lookup"><span data-stu-id="64c5a-106">site collection</span></span>
- <span data-ttu-id="64c5a-107">Oldalon</span><span class="sxs-lookup"><span data-stu-id="64c5a-107">site</span></span>
- <span data-ttu-id="64c5a-108">Lista</span><span class="sxs-lookup"><span data-stu-id="64c5a-108">list</span></span>
- <span data-ttu-id="64c5a-109">Könyvtár</span><span class="sxs-lookup"><span data-stu-id="64c5a-109">library</span></span>

<span data-ttu-id="64c5a-110">Ezenkívül a modern által nem támogatott bizonyos funkciókat és testreszabásokat használó listák továbbra is automatikusan klasszikus módba váltanak.</span><span class="sxs-lookup"><span data-stu-id="64c5a-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="64c5a-111">2019. április 1-től a bérlői szint letiltásának folyamata elindul és folytatódik 2019. május 31-ig.</span><span class="sxs-lookup"><span data-stu-id="64c5a-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="64c5a-112">A bérlők letiltása miatt klasszikus módban lévő listák és tárak automatikusan átkerülnek a modern rendszerbe.</span><span class="sxs-lookup"><span data-stu-id="64c5a-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="64c5a-113">Ha klasszikus módra van szüksége, olvassa el a további információkat [itt](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) és a PnP Powershell utasítást [itt,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) amely leírja a ma a klasszikus mód használatához használható lehetőségeket és eszközöket.</span><span class="sxs-lookup"><span data-stu-id="64c5a-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
