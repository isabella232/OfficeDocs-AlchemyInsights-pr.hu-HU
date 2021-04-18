---
title: A SharePoint-gyökérwebhely törlése
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
- "9003017"
- "5727"
ms.openlocfilehash: 849c5c58ab4688130d71baffac8fe39eddf92f18
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815473"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="f9598-102">A SharePoint-gyökérwebhely törlése</span><span class="sxs-lookup"><span data-stu-id="f9598-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="f9598-103">A SharePoint-gyökérwebhely törlése **nem támogatott.**</span><span class="sxs-lookup"><span data-stu-id="f9598-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="f9598-104">Ha a gyökérwebhelyet már törölték, a felhasználók 404-es, „A fájl nem található“ hibaüzenetet fognak kapni, amikor megpróbálnak hozzáférni a webhelyhez.</span><span class="sxs-lookup"><span data-stu-id="f9598-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="f9598-105">A probléma megoldásához az új SharePoint Felügyeleti központból állítsa vissza a webhelyet azzal, hogy a [Törölt webhelyek](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) lapon kijelöli a gyökérwebhelyet, és a Visszaállítás lehetőségre kattint.</span><span class="sxs-lookup"><span data-stu-id="f9598-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="f9598-106">A gyökérwebhely törlése helyett használja a [webhely cseréje](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) lehetőséget az új SharePoint Felügyeleti központból a gyökérwebhely visszaállítása után.</span><span class="sxs-lookup"><span data-stu-id="f9598-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="f9598-107">További információért lásd: [A gyökérwebhely modernizálása](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="f9598-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>