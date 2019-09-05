---
title: Nem lehet törölni az elemeket a SharePoint vagy az OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748561"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="dd41c-102">Az elemek nem törölhetők</span><span class="sxs-lookup"><span data-stu-id="dd41c-102">Unable to delete items</span></span>

<span data-ttu-id="dd41c-103">Problémák vannak a SharePoint-elemek törlésével?</span><span class="sxs-lookup"><span data-stu-id="dd41c-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="dd41c-104">Mindig győződjön meg arról, hogy rendelkezik a [megfelelő engedélyekkel](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) az elem törléséhez, vagy ha a [webhelycsoport rendszergazdája](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) megkísérli eltávolítani az elemet.</span><span class="sxs-lookup"><span data-stu-id="dd41c-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="dd41c-105">Ellenőrizze, hogy nincs-e az [adatmegőrzési házirend](https://docs.microsoft.com/office365/securitycompliance/retention-policies) beállítása a elemen.</span><span class="sxs-lookup"><span data-stu-id="dd41c-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="dd41c-106">Győződjön meg arról, hogy az elemet nem egy másik felhasználó [vette ki](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) .</span><span class="sxs-lookup"><span data-stu-id="dd41c-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="dd41c-107">Végül, ügyintéző tud használ [SharePoint példa és üzelmek](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) melyik tartalmaz egy könyvtár-ból PowerShell követel amit enged ön-hoz előad összetett vezetés tettek mint kényszerít törlés makacs cikk.</span><span class="sxs-lookup"><span data-stu-id="dd41c-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="dd41c-108">PNP-fájl eltávolítása</span><span class="sxs-lookup"><span data-stu-id="dd41c-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="dd41c-109">PNP-mappa eltávolítása</span><span class="sxs-lookup"><span data-stu-id="dd41c-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="dd41c-110">PNP-listaelem eltávolítása</span><span class="sxs-lookup"><span data-stu-id="dd41c-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="dd41c-111">PNP-lista eltávolítása</span><span class="sxs-lookup"><span data-stu-id="dd41c-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="dd41c-112">PNP mező eltávolítása (oszlop)</span><span class="sxs-lookup"><span data-stu-id="dd41c-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)