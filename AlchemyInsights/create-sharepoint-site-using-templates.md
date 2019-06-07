---
title: A SharePoint Online webhely létrehozása
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753710"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="6b690-102">Sablonok használata SharePoint-webhelyek létrehozása</span><span class="sxs-lookup"><span data-stu-id="6b690-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="6b690-103">SharePoint-webhely sablonok olyan előre elkészített meghatározások körül üzleti célok figyelembe vételével tervezték.</span><span class="sxs-lookup"><span data-stu-id="6b690-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="6b690-104">További információért lásd [a sablonok létrehozása a SharePoint-webhelyek különböző típusú](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="6b690-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="6b690-105">Az alábbiakban néhány közös problémák/mentése egy webhely vagy lista vonatkozó sablonként a Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="6b690-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="6b690-106">**Webhelyen vagy a listában sablon gomb nem érhető el vagy nincs megadva**</span><span class="sxs-lookup"><span data-stu-id="6b690-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="6b690-107">A rendszergazdák egyéni parancsfájl lehetővé kell sablon szolgáltatásainak használatához.</span><span class="sxs-lookup"><span data-stu-id="6b690-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="6b690-108">Részletes leírást, példák és szempontok:</span><span class="sxs-lookup"><span data-stu-id="6b690-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="6b690-109">Engedélyezhetjük vagy letilthatjuk az egyéni parancsfájl</span><span class="sxs-lookup"><span data-stu-id="6b690-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="6b690-110">A mentési hely sablon parancs nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúra webhelyeket.</span><span class="sxs-lookup"><span data-stu-id="6b690-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="6b690-111">A webhelysablon nem hozható létre vagy nem működik megfelelően.</span><span class="sxs-lookup"><span data-stu-id="6b690-111">The site template cannot be created or does not work correctly.</span></span>

<span data-ttu-id="6b690-112">A sablon [funkció](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) hiányzik, és nem aktiválható.</span><span class="sxs-lookup"><span data-stu-id="6b690-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="6b690-113">Ha a szolgáltatás nem érhető el az aktuális webhelycsoportban aktiválása, a webhelysablon webhelyet hozhat létre, nem használható.</span><span class="sxs-lookup"><span data-stu-id="6b690-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="6b690-114">Ellenőrizze, hogy ha a listák vagy tárak nagyobb a [Listanézet küszöbén korlát](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 cikkek, webhelysablon létrehozásának blokkolni tudja.</span><span class="sxs-lookup"><span data-stu-id="6b690-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="6b690-115">Előfordulhat, hogy a webhely használja túl sok erőforrást, és ezért a webhelysablon meghaladja az 50 MB-os korlátot.</span><span class="sxs-lookup"><span data-stu-id="6b690-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="6b690-116">Keresőoszlop használó listát származó adatokat megjelenítő problémák léptek fel.</span><span class="sxs-lookup"><span data-stu-id="6b690-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="6b690-117">További tudnivalókért tanulmányozza a [sablon által létrehozott listán nem jeleníti meg a megfelelő keresési lista a SharePoint Online adatait](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="6b690-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="6b690-118">Részletes információt a közös problémák és megoldások ellenőrizze a [webhely sablonok létrehozása és használata](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="6b690-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



