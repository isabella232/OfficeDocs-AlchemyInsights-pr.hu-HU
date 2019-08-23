---
title: Webhely vagy lista mentése sablonként
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: a74d14f1743b9a016346f7bf0943523b1ab21f91
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551633"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="9c5ec-102">Webhely vagy lista mentése sablonként</span><span class="sxs-lookup"><span data-stu-id="9c5ec-102">Save site or list as a template</span></span>

<span data-ttu-id="9c5ec-103">SharePoint-webhely sablonok olyan előre elkészített meghatározások körül üzleti célok figyelembe vételével tervezték.</span><span class="sxs-lookup"><span data-stu-id="9c5ec-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="9c5ec-104">További információért lásd [a sablonok létrehozása a SharePoint-webhelyek különböző típusú](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="9c5ec-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="9c5ec-105">Az alábbiakban néhány közös problémák/mentése egy webhely vagy lista vonatkozó sablonként a SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="9c5ec-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="9c5ec-106">**Mentés webhelyen vagy a listában sablon gomb nem elérhető vagy hiányzik**.</span><span class="sxs-lookup"><span data-stu-id="9c5ec-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="9c5ec-107">A rendszergazdák egyéni parancsfájl lehetővé kell sablon szolgáltatásainak használatához.</span><span class="sxs-lookup"><span data-stu-id="9c5ec-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="9c5ec-108">Talál részletes leírást, példák és megfontolások [engedélyezése vagy tiltása egyéni parancsfájl](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="9c5ec-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="9c5ec-109">A mentési hely sablon parancs nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúra webhelyeket.</span><span class="sxs-lookup"><span data-stu-id="9c5ec-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="9c5ec-110">**A webhelysablon nem hozható létre vagy nem működik megfelelően**</span><span class="sxs-lookup"><span data-stu-id="9c5ec-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="9c5ec-111">A sablon [funkció](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) hiányzik, és nem aktiválható.</span><span class="sxs-lookup"><span data-stu-id="9c5ec-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="9c5ec-112">Ha a szolgáltatás nem érhető el az aktuális webhelycsoportban aktiválása, a webhelysablon webhelyet hozhat létre, nem használható.</span><span class="sxs-lookup"><span data-stu-id="9c5ec-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="9c5ec-113">Ellenőrizze, hogy ha a listák vagy tárak nagyobb a [Listanézet küszöbén korlát](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 cikkek, webhelysablon létrehozásának blokkolni tudja.</span><span class="sxs-lookup"><span data-stu-id="9c5ec-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="9c5ec-114">Előfordulhat, hogy a webhely használja túl sok erőforrást, és ezért a webhelysablon meghaladja az 50 megabájt (MB).</span><span class="sxs-lookup"><span data-stu-id="9c5ec-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="9c5ec-115">Keresőoszlop használó listát származó adatokat megjelenítő problémák léptek fel.</span><span class="sxs-lookup"><span data-stu-id="9c5ec-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="9c5ec-116">További tudnivalókért tanulmányozza a [sablon által létrehozott listán nem jeleníti meg a megfelelő keresési lista a SharePoint Online adatait](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="9c5ec-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="9c5ec-117">További részletes információt a közös problémák és megoldások hivatkozás [létrehozása és használata a webhelysablonok](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)olvassa.</span><span class="sxs-lookup"><span data-stu-id="9c5ec-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

