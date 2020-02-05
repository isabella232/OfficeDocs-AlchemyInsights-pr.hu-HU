---
title: Webhely létrehozása a SharePoint Online-ban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770425"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="c94fd-102">SharePoint-webhelyek létrehozása sablonok használatával</span><span class="sxs-lookup"><span data-stu-id="c94fd-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="c94fd-103">A modern kommunikációs vagy csoportwebhelyek nem támogatják a webhely sablonként való mentését.</span><span class="sxs-lookup"><span data-stu-id="c94fd-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="c94fd-104">A sablonok használatáról további információt [a SharePoint-webhely mentése, letöltése és feltöltése sablonként](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="c94fd-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="c94fd-105">Íme néhány gyakori probléma/megoldás a Webhely vagy lista sharepoint online sablonként való mentésével kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="c94fd-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="c94fd-106">**Webhely/listasablon mentése gomb nem érhető el vagy hiányzik**</span><span class="sxs-lookup"><span data-stu-id="c94fd-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="c94fd-107">A rendszergazdáknak engedélyeznie kell az egyéni parancsfájlt a sablon szolgáltatásainak engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="c94fd-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="c94fd-108">A részletes lépésekről, példákról és szempontokról lásd:</span><span class="sxs-lookup"><span data-stu-id="c94fd-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="c94fd-109">Egyéni parancsfájl engedélyezése vagy lemegakadályozása</span><span class="sxs-lookup"><span data-stu-id="c94fd-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="c94fd-110">A Webhely mentése sablonként parancs nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúráját használó webhelyeken.</span><span class="sxs-lookup"><span data-stu-id="c94fd-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="c94fd-111">**A webhelysablon nem hozható létre, vagy nem működik megfelelően**</span><span class="sxs-lookup"><span data-stu-id="c94fd-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="c94fd-112">Lehet, hogy a sablonból hiányzik egy [szolgáltatás,](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) és nem aktiválódik.</span><span class="sxs-lookup"><span data-stu-id="c94fd-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="c94fd-113">Ha a funkció nem aktiválható az aktuális webhelycsoportban, a webhelysablon nem használható webhely létrehozására.</span><span class="sxs-lookup"><span data-stu-id="c94fd-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="c94fd-114">Ellenőrizze, hogy a listák vagy tárak túllépik-e az 5000-es [listakorlát-korlátot,](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) mivel ez letilthatja a webhelysablon létrehozását.</span><span class="sxs-lookup"><span data-stu-id="c94fd-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="c94fd-115">Lehet, hogy a webhely túl sok erőforrást használ, ezért a webhelysablon meghaladja az 50 MB-os korlátot.</span><span class="sxs-lookup"><span data-stu-id="c94fd-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="c94fd-116">Probléma merül fel a keresoszlopot használó listából származó adatok megjelenítése korával kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="c94fd-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="c94fd-117">További információt a Sablon által létrehozott lista nem [jelenít meg a SharePoint Online megfelelő keresőlistájának adatait.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)</span><span class="sxs-lookup"><span data-stu-id="c94fd-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="c94fd-118">A gyakori problémákról és megoldásokról további információt a Webhelysablonok létrehozása és használata című, a [webhelysablonok létrehozása című,](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)a</span><span class="sxs-lookup"><span data-stu-id="c94fd-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



