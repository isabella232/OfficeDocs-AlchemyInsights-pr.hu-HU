---
title: Webhely létrehozása a SharePoint Online szolgáltatásban
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755310"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="ac6a6-102">SharePoint-webhelyek létrehozása sablonokkal</span><span class="sxs-lookup"><span data-stu-id="ac6a6-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="ac6a6-103">A SharePoint webhelysablonok előre elkészített definíciók, amelyeket egy adott üzleti szükséglet köré terveztek.</span><span class="sxs-lookup"><span data-stu-id="ac6a6-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="ac6a6-104">További információ: [sablonok használata különféle SharePoint-webhelyek létrehozásához](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="ac6a6-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="ac6a6-105">Íme néhány gyakori probléma/megoldás a webhelyek vagy listák mentése sablonként a SharePoint Online szolgáltatásban.</span><span class="sxs-lookup"><span data-stu-id="ac6a6-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="ac6a6-106">**A webhely/listasablon mentése gomb nem érhető el vagy hiányzik**</span><span class="sxs-lookup"><span data-stu-id="ac6a6-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="ac6a6-107">A rendszergazdáknak az egyéni parancsfájl engedélyezése lehetőséget kell engedélyezni a sablonszolgáltatások engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="ac6a6-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="ac6a6-108">A részletes lépésekről, a példákat és megfontolásokat lásd:</span><span class="sxs-lookup"><span data-stu-id="ac6a6-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="ac6a6-109">Egyéni parancsfájl engedélyezése vagy tiltása</span><span class="sxs-lookup"><span data-stu-id="ac6a6-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="ac6a6-110">A webhely mentése sablonként parancs használata nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúrát használó webhelyeken.</span><span class="sxs-lookup"><span data-stu-id="ac6a6-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="ac6a6-111">**A webhelysablon nem hozható létre vagy nem működik megfelelően**</span><span class="sxs-lookup"><span data-stu-id="ac6a6-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="ac6a6-112">Lehet, hogy hiányzik egy [szolgáltatás](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , és a sablon nem aktiválható.</span><span class="sxs-lookup"><span data-stu-id="ac6a6-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="ac6a6-113">Ha a szolgáltatás nem aktiválható az aktuális webhelycsoportban, a webhelysablonnal nem lehet webhelyet létrehozni.</span><span class="sxs-lookup"><span data-stu-id="ac6a6-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="ac6a6-114">Ellenőriz-hoz lát ha akármi tetszik vagy könyvtárak kimagaslik a [oldalra dől kilátás korlátoz küszöb](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) -ból 5000 cikk mint ez tud fatuskó teremtés-ból egy telek mintadeszka.</span><span class="sxs-lookup"><span data-stu-id="ac6a6-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="ac6a6-115">Előfordulhat, hogy a webhely túl sok erőforrást használ, ezért a webhelysablon túllépi a 50 MB-os korlátot.</span><span class="sxs-lookup"><span data-stu-id="ac6a6-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="ac6a6-116">Problémák merülnek fel a keresőoszlopot használó listák adatainak megjelenítésekor.</span><span class="sxs-lookup"><span data-stu-id="ac6a6-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="ac6a6-117">További információ: [a sablon által generált lista nem jeleníti meg a SharePoint Online megfelelő keresőlistájából származó adatokat](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="ac6a6-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="ac6a6-118">A gyakori problémákról és megoldásokról a [webhelysablonok létrehozása és használata című oldalon](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)olvashat részletesebben.</span><span class="sxs-lookup"><span data-stu-id="ac6a6-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



