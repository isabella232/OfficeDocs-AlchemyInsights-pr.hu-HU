---
title: Nem lehet törölni a SharePoint- vagy OneDrive cikkek
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057724"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="ef34c-102">Nem törölhető elemek</span><span class="sxs-lookup"><span data-stu-id="ef34c-102">Unable to delete items</span></span>

<span data-ttu-id="ef34c-103">Elemek törlése a probléma?</span><span class="sxs-lookup"><span data-stu-id="ef34c-103">Having issues deleting items?</span></span>

- <span data-ttu-id="ef34c-104">Mindig ellenőrizze, hogy rendelkezik a [megfelelő engedélyekkel](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) , illetve törli az elemet a [webhelycsoport rendszergazdája](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) kísérlet eltávolítja az elemet.</span><span class="sxs-lookup"><span data-stu-id="ef34c-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="ef34c-105">Győződjön meg arról, hogy nincs olyan [adatmegőrzési szabály](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) beállítása az elemen.</span><span class="sxs-lookup"><span data-stu-id="ef34c-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="ef34c-106">Ellenőrizze, hogy az elem nem egy másik felhasználó [kivette](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) .</span><span class="sxs-lookup"><span data-stu-id="ef34c-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="ef34c-107">Végül a rendszergazdák használhatják [SharePoint szokások és gyakorlatok](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) tartalmazó könyvtár PowerShell parancsok, amelyek lehetővé teszik az összetett kezelési műveletek végrehajtásához kényszerítése stubborn elemek törlése.</span><span class="sxs-lookup"><span data-stu-id="ef34c-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="ef34c-108">PNP fájl eltávolítása</span><span class="sxs-lookup"><span data-stu-id="ef34c-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="ef34c-109">PNP-mappa eltávolítása</span><span class="sxs-lookup"><span data-stu-id="ef34c-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="ef34c-110">Távolítsa el a PNP listaelem</span><span class="sxs-lookup"><span data-stu-id="ef34c-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="ef34c-111">PNP lista törlése</span><span class="sxs-lookup"><span data-stu-id="ef34c-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="ef34c-112">Távolítsa el a PNP mező (oszlop)</span><span class="sxs-lookup"><span data-stu-id="ef34c-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)