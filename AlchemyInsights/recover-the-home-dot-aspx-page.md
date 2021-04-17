---
title: A home.aspx lap helyreállítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002970"
- "5683"
ms.openlocfilehash: e235e7d29935dd9fa6e0c286dbe053e76d08c64e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51800099"
---
# <a name="recover-the-homeaspx-page"></a><span data-ttu-id="e63d9-102">A home.aspx lap helyreállítása</span><span class="sxs-lookup"><span data-stu-id="e63d9-102">Recover the Home.aspx page</span></span>

<span data-ttu-id="e63d9-103">Ha törli a webhely kezdőlapját, a Lomtárból visszaállíthatja a Lomtár-hivatkozáson keresztül.</span><span class="sxs-lookup"><span data-stu-id="e63d9-103">If the site home page is deleted, it can be recovered from the Recycle Bin by accessing the Recycle Bin URL.</span></span>

1. <span data-ttu-id="e63d9-104">Nyissa meg a https://\<tenantname>.sharepoint.com/sites/\<sitename>/_layouts/15/RecycleBin.aspx? lapot úgy, hogy helyettesíti a<**bérlőnevet**> a bérlője nevével és a <**webhelynevet**> a webhelye nevével.</span><span class="sxs-lookup"><span data-stu-id="e63d9-104">Navigate to https://\<tenantname>.sharepoint.com/sites/\<sitename>/_layouts/15/RecycleBin.aspx?, by replacing <**tenantname**> with the name of your tenant and <**sitename**> with the name of your site.</span></span>

2. <span data-ttu-id="e63d9-105">Válassza ki a visszaállítani kívánt lapot.</span><span class="sxs-lookup"><span data-stu-id="e63d9-105">Select the page to restore.</span></span>

<span data-ttu-id="e63d9-106">Ha a kezdőlap továbbra sem található, létrehozhat egy új lapot a webhelyen, [ amelyet megadhat a webhely kezdőlapjaként](https://support.microsoft.com/en-gb/office/use-a-different-page-for-your-sharepoint-site-home-page-35a5022c-f84a-455d-985e-c691ab5dfa17?ui=en-us&rs=en-gb&ad=gb).</span><span class="sxs-lookup"><span data-stu-id="e63d9-106">If the home page still cannot be found, you can create a new site page and [set it as your site home page](https://support.microsoft.com/en-gb/office/use-a-different-page-for-your-sharepoint-site-home-page-35a5022c-f84a-455d-985e-c691ab5dfa17?ui=en-us&rs=en-gb&ad=gb).</span></span> <span data-ttu-id="e63d9-107">A 404-es (nem található) hiba nem jelenik meg többé a webhely elérésekor.</span><span class="sxs-lookup"><span data-stu-id="e63d9-107">The 404 not found error should no longer appear when you try to access the site.</span></span>
