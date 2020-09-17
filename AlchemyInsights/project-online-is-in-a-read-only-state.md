---
title: A Project online írásvédett állapotban van
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801654"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="66f04-102">A Project online írásvédett állapotban van</span><span class="sxs-lookup"><span data-stu-id="66f04-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="66f04-103">Három általános oka lehet annak, hogy a Project online csak olvasható állapotot érhet el:</span><span class="sxs-lookup"><span data-stu-id="66f04-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="66f04-104">A szervezeteknek csak Project online Essentials licenccel (s) kell rendelkezniük.</span><span class="sxs-lookup"><span data-stu-id="66f04-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="66f04-105">Ez nem elegendő ahhoz, hogy a webhely életben maradjon, és az előbbi használatba kerül.</span><span class="sxs-lookup"><span data-stu-id="66f04-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="66f04-106">Egy írásvédett államba tesszük a webhelyet, hogy a rendszergazdák tudják, hogy valami nem stimmel, és a megfelelő licencek is megszerezhetők.</span><span class="sxs-lookup"><span data-stu-id="66f04-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="66f04-107">A rendszergazdáknak létre kell hozniuk egy Project online Professional-és/vagy prémium licencet.</span><span class="sxs-lookup"><span data-stu-id="66f04-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="66f04-108">A webhely ekkor már csak olvasható.</span><span class="sxs-lookup"><span data-stu-id="66f04-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="66f04-109">További információt a [projektvezetési megoldások összehasonlítása](https://products.office.com/project/compare-microsoft-project-management-software?tab=1)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="66f04-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="66f04-110">Elérte a hozzárendelt kvótát.</span><span class="sxs-lookup"><span data-stu-id="66f04-110">Assigned quota has been reached.</span></span> <span data-ttu-id="66f04-111">További információt a [Project Web App-kvóta](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="66f04-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="66f04-112">Ellenőrizze, hogy a [Project online időfázisos jelentéskészítési adatainak összesítését szeretné-](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) e ellenőrizni, hogy miként befolyásolhatják a jelentések részletességét.</span><span class="sxs-lookup"><span data-stu-id="66f04-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="66f04-113">Írásvédett lehet nagyon ideiglenes feltétel, amely a karbantartás során is bekövetkezhet.</span><span class="sxs-lookup"><span data-stu-id="66f04-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="66f04-114">Ügyfeleink a legtöbb karbantartást még észre sem veszik, és nem fogja látni ezt, de vannak olyan esetek, amikor a rövid idő csak olvasható.</span><span class="sxs-lookup"><span data-stu-id="66f04-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
