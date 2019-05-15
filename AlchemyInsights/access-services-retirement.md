---
title: Access services nyugdíjazás
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973924"
---
# <a name="access-services-retirement"></a><span data-ttu-id="67370-102">Access services nyugdíjazás</span><span class="sxs-lookup"><span data-stu-id="67370-102">Access services retirement</span></span>

<span data-ttu-id="67370-103">Azt eredetileg meghirdetik március 2017, MC97576, és továbbra is kommunikálni az elmúlt év az Office 365 szolgáltatásainak eléréséhez van hatókörről.</span><span class="sxs-lookup"><span data-stu-id="67370-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="67370-104">A következő fázis a folyamat alapjául szolgáló adatok tárolására használja a SharePoint-listák Access webes adatbázisok eltávolítása lesz.</span><span class="sxs-lookup"><span data-stu-id="67370-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="67370-105">Hogyan ez befolyásolja nekem?</span><span class="sxs-lookup"><span data-stu-id="67370-105">How does this affect me?</span></span>

<span data-ttu-id="67370-106">Június 2019 kezdődően azt leállítja a SharePoint Online új Access-adatbázisok létrehozása és állítsa le a szolgáltatás és a fennmaradó apps április 2020-ra történő.</span><span class="sxs-lookup"><span data-stu-id="67370-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="67370-107">Mit kell tennem a módosítás előkészítése?</span><span class="sxs-lookup"><span data-stu-id="67370-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="67370-108">Javasoljuk, hogy a szervezet webes adatbázisokat az átállási terv létrehozása.</span><span class="sxs-lookup"><span data-stu-id="67370-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="67370-109">Rendszergazdák a [hozzáférést a SharePoint app képolvasó](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) segítségével szerezze be az Access apps helyek használó leltárt.</span><span class="sxs-lookup"><span data-stu-id="67370-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="67370-110">Számos módon át az Access webes adatbázisok adatok:</span><span class="sxs-lookup"><span data-stu-id="67370-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="67370-111">Egy helyi Access adatbázist importál (. ACCDB) vagy Excel-fájl.</span><span class="sxs-lookup"><span data-stu-id="67370-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="67370-112">Szintén ajánlott alternatív platformjának kódot nem üzleti megoldásokat a webes és mobil eszközök, a Microsoft PowerApps felfedezése.</span><span class="sxs-lookup"><span data-stu-id="67370-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>