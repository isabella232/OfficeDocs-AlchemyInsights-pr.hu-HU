---
title: Webhely létrehozása a SharePoint Online-ban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732228"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="f87e7-102">SharePoint-webhelyek létrehozása sablonok használatával</span><span class="sxs-lookup"><span data-stu-id="f87e7-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="f87e7-103">A webhelyek sablonként való mentésének lehetőségét a modern kommunikációs vagy csoportwebhely-webhelyek nem támogatják.</span><span class="sxs-lookup"><span data-stu-id="f87e7-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="f87e7-104">A sablonok használatáról további információt a [SharePoint-webhely mentése, letöltése és feltöltése sablonként](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="f87e7-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="f87e7-105">Az alábbiakban néhány gyakori problémát és megoldást találhat a webhelyek vagy listák sablonként való mentésekor a SharePoint Online-ban.</span><span class="sxs-lookup"><span data-stu-id="f87e7-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="f87e7-106">**A webhely/lista sablonjának mentése gomb nem érhető el vagy hiányzik**</span><span class="sxs-lookup"><span data-stu-id="f87e7-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="f87e7-107">A rendszergazdáknak engedélyezniük kell az egyéni parancsfájlok számára a sablonok funkcióinak használatát.</span><span class="sxs-lookup"><span data-stu-id="f87e7-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="f87e7-108">A lépések részletes ismertetése:</span><span class="sxs-lookup"><span data-stu-id="f87e7-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="f87e7-109">Egyéni parancsfájlok engedélyezése vagy letiltása</span><span class="sxs-lookup"><span data-stu-id="f87e7-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="f87e7-110">A webhely mentése sablonként parancs nem érhető el, és problémákat okozhat a SharePoint Server közzétételi infrastruktúráját használó webhelyeken.</span><span class="sxs-lookup"><span data-stu-id="f87e7-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="f87e7-111">**A webhelysablon nem hozható létre vagy nem működik megfelelően**</span><span class="sxs-lookup"><span data-stu-id="f87e7-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="f87e7-112">Előfordulhat, hogy a sablon hiányzik egy [funkcióból](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , és nem aktiválódik.</span><span class="sxs-lookup"><span data-stu-id="f87e7-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="f87e7-113">Ha a funkció nem érhető el az aktuális webhelycsoportban, a webhelysablonok nem használhatók webhelyek létrehozására.</span><span class="sxs-lookup"><span data-stu-id="f87e7-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="f87e7-114">Ellenőrizze, hogy a lista vagy a tárak túllépik-e az 5000-elemek [listanézet-küszöbértékét](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , mivel ez letilthatja a webhelysablon létrehozását.</span><span class="sxs-lookup"><span data-stu-id="f87e7-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="f87e7-115">Előfordulhat, hogy a webhely túl sok erőforrást használ, ezért a webhelysablon túllépi a 50 MB-os korlátot.</span><span class="sxs-lookup"><span data-stu-id="f87e7-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="f87e7-116">Problémák vannak az olyan listákban, amelyek keresési oszlopot használnak.</span><span class="sxs-lookup"><span data-stu-id="f87e7-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="f87e7-117">További információ: [a sablonok által generált lista nem jeleníti meg az adatokat a SharePoint Online-ban a megfelelő keresési listából](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="f87e7-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="f87e7-118">A gyakori problémákról és megoldásokról további információt a [webhelysablonok létrehozása és használata](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="f87e7-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



