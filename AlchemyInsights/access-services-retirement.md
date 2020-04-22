---
title: Hozzáférés szolgáltatások nyugdíjazás
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687260"
---
# <a name="access-services-retirement"></a><span data-ttu-id="bdb5b-102">Hozzáférés szolgáltatások nyugdíjazás</span><span class="sxs-lookup"><span data-stu-id="bdb5b-102">Access services retirement</span></span>

<span data-ttu-id="bdb5b-103">Ahogy azt eredetileg az MC97576-ban, 2017 márciusában jelentettük be, és az elmúlt évben folytattuk a kommunikációt, az Access Services-t megszüntették.</span><span class="sxs-lookup"><span data-stu-id="bdb5b-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="bdb5b-104">A folyamat következő fázisa az Access webadatbázisok eltávolítása lesz, amelyek a SharePoint-listákat használják alapul szolgáló adattárolóként.</span><span class="sxs-lookup"><span data-stu-id="bdb5b-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="bdb5b-105">**Milyen hatással van ez rám?**</span><span class="sxs-lookup"><span data-stu-id="bdb5b-105">**How does this affect me?**</span></span>

<span data-ttu-id="bdb5b-106">2019 júniusátantól leállítjuk az új Access-adatbázisok létrehozását a SharePoint Online-ban, és 2020 áprilisáig leállítjuk a szolgáltatást és a többi alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="bdb5b-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="bdb5b-107">**Mit kell tennem, hogy felkészüljek erre a változásra?**</span><span class="sxs-lookup"><span data-stu-id="bdb5b-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="bdb5b-108">Javasoljuk, hogy hozzon létre egy átmeneti tervet a szervezet Access webes adatbázisaihoz.</span><span class="sxs-lookup"><span data-stu-id="bdb5b-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="bdb5b-109">A rendszergazdák a [SharePoint Access alkalmazásképolvasó](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) segítségével leltárt kaphatnak a webhelyek által használt Access-alkalmazásokról.</span><span class="sxs-lookup"><span data-stu-id="bdb5b-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="bdb5b-110">Az Access webes adatbázisok adatainak áttelepítése többféleképpen is elérhető:</span><span class="sxs-lookup"><span data-stu-id="bdb5b-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="bdb5b-111">Importálás helyi Access adatbázisba (. ACCDB) vagy egy Excel-fájlba.</span><span class="sxs-lookup"><span data-stu-id="bdb5b-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="bdb5b-112">Azt is javasoljuk, hogy vizsgálja meg a Microsoft PowerApps-et alternatív platformként, hogy kód nélküli üzleti megoldásokat hozzon létre webes és mobileszközökhöz.</span><span class="sxs-lookup"><span data-stu-id="bdb5b-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>