---
title: Ez a webhely nem érhető el – hiba a SharePoint-webhely böngészőből vagy Teamsből való elérésekor
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 451544fb85522e0eececc9274825805699685ee9
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744980"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a><span data-ttu-id="f72da-102">"Ez a webhely nem érhető el" hibaüzenet jelenik meg, amikor megpróbál hozzáférni a SharePoint-webhelyhez a böngészőből vagy a Teamsből</span><span class="sxs-lookup"><span data-stu-id="f72da-102">“This site can’t be reached” error when trying to access SharePoint site from browser or Teams</span></span>

<span data-ttu-id="f72da-103">Amikor a felhasználók böngészőből vagy Teamsből próbálnak hozzáférni a SharePoint-webhelyhez, a "Nem érhető el a webhely" hibaüzenet jelenhet meg.</span><span class="sxs-lookup"><span data-stu-id="f72da-103">Users might receive "This site can't be reached" error when trying to access SharePoint site from browser or Teams.</span></span> 

<span data-ttu-id="f72da-104">A probléma megoldása:</span><span class="sxs-lookup"><span data-stu-id="f72da-104">To resolve this issue:</span></span> 

1. <span data-ttu-id="f72da-105">Ellenőrizze, hogy a kezdőlap a Lomtárban vagy a másodszakaszban lévő lomtárban van-e, és állítsa vissza a lapot.</span><span class="sxs-lookup"><span data-stu-id="f72da-105">Check if the home page is in Recycle bin or second-stage recycle bin and restore the page.</span></span>

<span data-ttu-id="f72da-106">**Példa a lomtár közvetlen URL-címére:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="f72da-106">**Sample direct URL to recycle bin**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>

1. <span data-ttu-id="f72da-107">Ha a kezdőlapot véglegesen eltávolítja a lomtárból, hozzon létre egy új webhelyet a Webhelylapok tárból, és tegye kezdőlapként.</span><span class="sxs-lookup"><span data-stu-id="f72da-107">If the home page is permanently removed from the recycle bin, create a new site page from the Site Pages library and make it a homepage.</span></span> 

<span data-ttu-id="f72da-108">**Közvetlen URL-minta:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="f72da-108">**Sample direct URL**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>