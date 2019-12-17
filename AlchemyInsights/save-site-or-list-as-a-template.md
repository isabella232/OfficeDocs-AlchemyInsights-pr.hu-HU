---
title: Webhely vagy lista mentése sablonként
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048726"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="ef9fa-102">Webhely vagy lista mentése sablonként</span><span class="sxs-lookup"><span data-stu-id="ef9fa-102">Save site or list as a template</span></span>

<span data-ttu-id="ef9fa-103">A SharePoint webhelysablonok előre elkészített definíciók, amelyeket egy adott üzleti szükséglet köré terveztek.</span><span class="sxs-lookup"><span data-stu-id="ef9fa-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="ef9fa-104">További információ: [sablonok használata különféle SharePoint-webhelyek létrehozásához](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="ef9fa-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="ef9fa-105">Íme néhány gyakori probléma/megoldás a webhelyek vagy listák mentése sablonként a SharePoint Online szolgáltatásban.</span><span class="sxs-lookup"><span data-stu-id="ef9fa-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="ef9fa-106">**A webhely/listasablon mentése gomb nem érhető el vagy hiányzik**.</span><span class="sxs-lookup"><span data-stu-id="ef9fa-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="ef9fa-107">A rendszergazdáknak az egyéni parancsfájl engedélyezése lehetőséget kell engedélyezni a sablonszolgáltatások engedélyezéséhez.</span><span class="sxs-lookup"><span data-stu-id="ef9fa-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="ef9fa-108">A részletes lépésekről példákat és megfontolásokat az [egyéni parancsfájl engedélyezése vagy tiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="ef9fa-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="ef9fa-109">A webhely mentése sablonként parancs használata nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúrát használó webhelyeken.</span><span class="sxs-lookup"><span data-stu-id="ef9fa-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="ef9fa-110">**A webhelysablon nem hozható létre vagy nem működik megfelelően**</span><span class="sxs-lookup"><span data-stu-id="ef9fa-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="ef9fa-111">Lehet, hogy hiányzik egy [szolgáltatás](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , és a sablon nem aktiválható.</span><span class="sxs-lookup"><span data-stu-id="ef9fa-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="ef9fa-112">Ha a szolgáltatás nem aktiválható az aktuális webhelycsoportban, a webhelysablonnal nem lehet webhelyet létrehozni.</span><span class="sxs-lookup"><span data-stu-id="ef9fa-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="ef9fa-113">Ellenőriz-hoz lát ha akármi tetszik vagy könyvtárak kimagaslik a [oldalra dől kilátás korlátoz küszöb](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) -ból 5000 cikk mint ez tud fatuskó teremtés-ból egy telek mintadeszka.</span><span class="sxs-lookup"><span data-stu-id="ef9fa-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="ef9fa-114">Elképzelhető, hogy a webhely túl sok erőforrást használ, ezért a webhelysablon túllépi az 50 megabájt (MB) korlátot.</span><span class="sxs-lookup"><span data-stu-id="ef9fa-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="ef9fa-115">Problémák merülnek fel a keresőoszlopot használó listák adatainak megjelenítésekor.</span><span class="sxs-lookup"><span data-stu-id="ef9fa-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="ef9fa-116">További információ: [a sablon által generált lista nem jeleníti meg a SharePoint Online megfelelő keresőlistájából származó adatokat](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="ef9fa-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="ef9fa-117">További részletes információ a közös problémákról és megoldásokért kérjük, [hozzon létre és használjon webhelysablonokat](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="ef9fa-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

