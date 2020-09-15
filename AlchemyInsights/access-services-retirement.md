---
title: Az Access Services nyugdíjazása
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698684"
---
# <a name="access-services-retirement"></a><span data-ttu-id="76273-102">Az Access Services nyugdíjazása</span><span class="sxs-lookup"><span data-stu-id="76273-102">Access services retirement</span></span>

<span data-ttu-id="76273-103">Ahogy azt eredetileg a MC97576-ban jelentették be, az 2017 márciusi verziójában továbbra is megszűnt a kommunikáció az elmúlt évi Access-szolgáltatásokkal.</span><span class="sxs-lookup"><span data-stu-id="76273-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="76273-104">A folyamat következő fázisa azokat az Access-webadatbázisokat fogja eltávolítani, amelyek a SharePoint-listákat használják a mögöttes adattárolóként.</span><span class="sxs-lookup"><span data-stu-id="76273-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="76273-105">**Milyen hatással van ez rám?**</span><span class="sxs-lookup"><span data-stu-id="76273-105">**How does this affect me?**</span></span>

<span data-ttu-id="76273-106">A 2019 júniusi verziójában az új Access-adatbázisok létrehozása megszűnik a SharePoint Online-ban, és április 2020-től leállíthatja a szolgáltatást és a fennmaradó alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="76273-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="76273-107">**Mit kell tennem, hogy felkészüljenek erre a változásra?**</span><span class="sxs-lookup"><span data-stu-id="76273-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="76273-108">Javasoljuk, hogy hozzon létre egy áttűnési tervet a szervezete Access-alapú webes adatbázisaihoz.</span><span class="sxs-lookup"><span data-stu-id="76273-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="76273-109">A rendszergazdák a [SharePoint Access app-szkenner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) segítségével beállíthatják a webhelyek által használt Access-alkalmazások leltárát.</span><span class="sxs-lookup"><span data-stu-id="76273-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="76273-110">Az Access-webadatbázisok adatainak áttelepítése többféle módon történik:</span><span class="sxs-lookup"><span data-stu-id="76273-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="76273-111">Importálás helyi Access-adatbázisba (. ACCDB) vagy egy Excel-fájlra.</span><span class="sxs-lookup"><span data-stu-id="76273-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="76273-112">Javasoljuk, hogy a Microsoft PowerApps-ot alternatív platformként vizsgálja meg, hogy a rendszer nem hoz létre a webes és mobileszközök számára a nem-kódolt üzleti megoldásokat.</span><span class="sxs-lookup"><span data-stu-id="76273-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>