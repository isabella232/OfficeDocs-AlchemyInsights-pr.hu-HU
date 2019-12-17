---
title: A SharePoint Online klasszikus üzemmódra korlátozása
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048762"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="536d6-102">A SharePoint Online klasszikus üzemmódra korlátozása</span><span class="sxs-lookup"><span data-stu-id="536d6-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="536d6-103">Egyes szervezeteknél továbbra is klasszikus üzemmódra van szükség.</span><span class="sxs-lookup"><span data-stu-id="536d6-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="536d6-104">Bár nem tervezi, hogy távolítsa el a klasszikus mód a szemcsés szinten, már nem lehet korlátozni egy egész szervezet (bérlő) a klasszikus mód listák és tárak.</span><span class="sxs-lookup"><span data-stu-id="536d6-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="536d6-105">A admin akarat volna a következő választások-hoz kezel egyén tetszik és könyvtárak-ban klasszikus mód használ szemcsés választ-ki kapcsol amit mi beszerez-nél alábbiak szintek:</span><span class="sxs-lookup"><span data-stu-id="536d6-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="536d6-106">webhelycsoport</span><span class="sxs-lookup"><span data-stu-id="536d6-106">site collection</span></span>
- <span data-ttu-id="536d6-107">Oldalon</span><span class="sxs-lookup"><span data-stu-id="536d6-107">site</span></span>
- <span data-ttu-id="536d6-108">Lista</span><span class="sxs-lookup"><span data-stu-id="536d6-108">list</span></span>
- <span data-ttu-id="536d6-109">Könyvtár</span><span class="sxs-lookup"><span data-stu-id="536d6-109">library</span></span>

<span data-ttu-id="536d6-110">Továbbá azok a listák, amelyek bizonyos szolgáltatásokat és testreszabásokat használnak, amelyeket a modern nem támogat, továbbra is automatikusan klasszikus módra lesznek átkapcsolva.</span><span class="sxs-lookup"><span data-stu-id="536d6-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="536d6-111">Kezdet április 1, 2019, a folyamat-hoz megbénít a bérlő szinten opt out a modern lista és könyvtárak indul, és továbbra is a május 31, 2019.</span><span class="sxs-lookup"><span data-stu-id="536d6-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="536d6-112">Azok a listák és könyvtárak, amelyek klasszikus módban vannak bérlő opt-out eredményeként automatikusan eltolódnak a modern.</span><span class="sxs-lookup"><span data-stu-id="536d6-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="536d6-113">Ha klasszikus üzemmódra van szüksége, olvassa el a további tudnivalókat [itt](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) , és a PnP PowerShell instrukció [itt](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) leírja azokat a lehetőségeket és eszközöket, amelyeket ma használhat a klasszikus üzemmód használatához.</span><span class="sxs-lookup"><span data-stu-id="536d6-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
