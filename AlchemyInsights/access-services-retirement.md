---
title: Access services nyugdíjazás
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495753"
---
# <a name="access-services-retirement"></a><span data-ttu-id="216e7-102">Access services nyugdíjazás</span><span class="sxs-lookup"><span data-stu-id="216e7-102">Access services retirement</span></span>

<span data-ttu-id="216e7-103">Azt eredetileg meghirdetik március 2017, MC97576, és továbbra is kommunikálni az elmúlt év az Office 365 szolgáltatásainak eléréséhez van hatókörről.</span><span class="sxs-lookup"><span data-stu-id="216e7-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="216e7-104">A következő fázis a folyamat alapjául szolgáló adatok tárolására használja a SharePoint-listák Access webes adatbázisok eltávolítása lesz.</span><span class="sxs-lookup"><span data-stu-id="216e7-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="216e7-105">**Hogyan ez befolyásolja nekem?**</span><span class="sxs-lookup"><span data-stu-id="216e7-105">**How does this affect me?**</span></span>

<span data-ttu-id="216e7-106">Június 2019 kezdődően azt leállítja a SharePoint Online új Access-adatbázisok létrehozása és állítsa le a szolgáltatás és a fennmaradó apps április 2020-ra történő.</span><span class="sxs-lookup"><span data-stu-id="216e7-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="216e7-107">**Mit kell tennem a módosítás előkészítése?**</span><span class="sxs-lookup"><span data-stu-id="216e7-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="216e7-108">Javasoljuk, hogy a szervezet webes adatbázisokat az átállási terv létrehozása.</span><span class="sxs-lookup"><span data-stu-id="216e7-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="216e7-109">Rendszergazdák a [hozzáférést a SharePoint app képolvasó](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) segítségével szerezze be az Access apps helyek használó leltárt.</span><span class="sxs-lookup"><span data-stu-id="216e7-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="216e7-110">Számos módon át az Access webes adatbázisok adatok:</span><span class="sxs-lookup"><span data-stu-id="216e7-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="216e7-111">Egy helyi Access adatbázist importál (. ACCDB) vagy Excel-fájl.</span><span class="sxs-lookup"><span data-stu-id="216e7-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="216e7-112">Szintén ajánlott alternatív platformjának kódot nem üzleti megoldásokat a webes és mobil eszközök, a Microsoft PowerApps felfedezése.</span><span class="sxs-lookup"><span data-stu-id="216e7-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>