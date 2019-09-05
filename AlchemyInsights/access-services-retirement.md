---
title: Hozzáférési szolgáltatások visszavonulása
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747786"
---
# <a name="access-services-retirement"></a><span data-ttu-id="9b64e-102">Hozzáférési szolgáltatások visszavonulása</span><span class="sxs-lookup"><span data-stu-id="9b64e-102">Access services retirement</span></span>

<span data-ttu-id="9b64e-103">Mint mi eredetileg jelentették be-ban MC97576, márciusban 2017, és állandó-hoz kommunikál felső a múlt év belépés szolgáltatás van lét nyugdíjas-ból Hivatal 365.</span><span class="sxs-lookup"><span data-stu-id="9b64e-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="9b64e-104">A folyamat következő fázisa az Access web adatbázisok eltávolítása lesz, amelyek a SharePoint-listákat a mögöttes adattárolásként használják.</span><span class="sxs-lookup"><span data-stu-id="9b64e-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="9b64e-105">**Hogyan érint ez engem?**</span><span class="sxs-lookup"><span data-stu-id="9b64e-105">**How does this affect me?**</span></span>

<span data-ttu-id="9b64e-106">Összerezzenés Június 2019, mi akarat megáll teremtés-ból új belépés adatbázisok-ban SharePoint Online és becsuk legyőz a szolgáltatás és akármi megmaradó Apps mellett április 2020.</span><span class="sxs-lookup"><span data-stu-id="9b64e-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="9b64e-107">**Mit kell tennem, hogy felkészüljünk erre a változra?**</span><span class="sxs-lookup"><span data-stu-id="9b64e-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="9b64e-108">Javasoljuk, hogy hozzon létre egy áttérési tervet a szervezet Access webes adatbázisaihoz.</span><span class="sxs-lookup"><span data-stu-id="9b64e-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="9b64e-109">Az adminisztrátorok használhatják a [SharePoint Access alkalmazás ellenőrzőszámát](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , hogy leltárt kapjanak a webhelyek által használt Access alkalmazásokról.</span><span class="sxs-lookup"><span data-stu-id="9b64e-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="9b64e-110">Az Access webadatbázisok adatainak áttelepítése többféle módon történjen:</span><span class="sxs-lookup"><span data-stu-id="9b64e-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="9b64e-111">Importálás helyi Access-adatbázisba (. ACCDB) vagy Excel-fájlba.</span><span class="sxs-lookup"><span data-stu-id="9b64e-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="9b64e-112">Mi is ajánl exploring Mikroszkóp PowerApps mint egy vagylagos emelvény-hoz teremt nem-kód teendő megoldások részére pókháló és mozgatható berendezés.</span><span class="sxs-lookup"><span data-stu-id="9b64e-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>