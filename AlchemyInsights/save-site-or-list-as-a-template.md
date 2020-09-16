---
title: Webhely vagy lista mentése sablonként
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727533"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="58080-102">Webhely vagy lista mentése sablonként</span><span class="sxs-lookup"><span data-stu-id="58080-102">Save site or list as a template</span></span>

<span data-ttu-id="58080-103">A SharePoint-webhelysablonok előre elkészített definíciók, amelyek egy adott üzleti szükséglet köré lettek tervezve.</span><span class="sxs-lookup"><span data-stu-id="58080-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="58080-104">További információt a [sablonok használata a különböző típusú SharePoint-webhelyek létrehozásához](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="58080-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="58080-105">Az alábbiakban néhány gyakori problémát és megoldást találhat a webhelyek vagy listák sablonként való mentésekor a SharePoint Online-ban.</span><span class="sxs-lookup"><span data-stu-id="58080-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="58080-106">**A webhely/lista sablonjának mentése gomb nem érhető el vagy hiányzik**.</span><span class="sxs-lookup"><span data-stu-id="58080-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="58080-107">A rendszergazdáknak engedélyezniük kell az egyéni parancsfájlok számára a sablonok funkcióinak használatát.</span><span class="sxs-lookup"><span data-stu-id="58080-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="58080-108">A lépések részletes ismertetését az [egyéni parancsfájlok engedélyezése vagy letiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)című témakörben találhatja meg.</span><span class="sxs-lookup"><span data-stu-id="58080-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="58080-109">A webhely mentése sablonként parancs nem érhető el, és problémákat okozhat a SharePoint Server közzétételi infrastruktúráját használó webhelyeken.</span><span class="sxs-lookup"><span data-stu-id="58080-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="58080-110">**A webhelysablon nem hozható létre vagy nem működik megfelelően**</span><span class="sxs-lookup"><span data-stu-id="58080-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="58080-111">Előfordulhat, hogy a sablon hiányzik egy [funkcióból](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , és nem aktiválódik.</span><span class="sxs-lookup"><span data-stu-id="58080-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="58080-112">Ha a funkció nem érhető el az aktuális webhelycsoportban, a webhelysablonok nem használhatók webhelyek létrehozására.</span><span class="sxs-lookup"><span data-stu-id="58080-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="58080-113">Ellenőrizze, hogy a lista vagy a tárak túllépik-e az 5000-elemek [listanézet-küszöbértékét](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , mivel ez letilthatja a webhelysablon létrehozását.</span><span class="sxs-lookup"><span data-stu-id="58080-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="58080-114">Előfordulhat, hogy a webhely túl sok erőforrást használ, ezért a webhelysablon túllépi a 50 megabájtos (MB) korlátját.</span><span class="sxs-lookup"><span data-stu-id="58080-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="58080-115">Problémák vannak az olyan listákban, amelyek keresési oszlopot használnak.</span><span class="sxs-lookup"><span data-stu-id="58080-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="58080-116">További információ: [a sablonok által generált lista nem jeleníti meg az adatokat a SharePoint Online-ban a megfelelő keresési listából](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="58080-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="58080-117">A gyakori problémákról és megoldásokról további információt a [webhelysablonok létrehozása és használata](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="58080-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

