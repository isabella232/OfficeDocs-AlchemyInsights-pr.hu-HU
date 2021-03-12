---
title: A SharePoint-gyökérwebhely törlése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: d33029b6fe333b38cee7dba66ba4a5044248f174
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713816"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="1caeb-102">A SharePoint-gyökérwebhely törlése</span><span class="sxs-lookup"><span data-stu-id="1caeb-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="1caeb-103">A SharePoint-gyökérwebhely törlése  **nem támogatott.**</span><span class="sxs-lookup"><span data-stu-id="1caeb-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="1caeb-104">Ha a gyökérwebhely már törölve van, a felhasználók a 404-es fájl nem található hibaüzenetet fogják tapasztalni a webhely elérésekor.</span><span class="sxs-lookup"><span data-stu-id="1caeb-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="1caeb-105">A probléma megoldásához állítsa vissza a webhelyet az [](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) új SharePoint Felügyeleti központból a Törölt webhelyek lapra kattintva, jelölje ki a gyökérwebhelyet, és kattintson a Visszaállítás gombra.</span><span class="sxs-lookup"><span data-stu-id="1caeb-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="1caeb-106">A gyökérwebhely törlése helyett [](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) használja az új SharePoint Felügyeleti központ cserewebhelyét a gyökérwebhely visszaállítása után.</span><span class="sxs-lookup"><span data-stu-id="1caeb-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="1caeb-107">További információt a [gyökérwebhely modernizálása](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="1caeb-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>