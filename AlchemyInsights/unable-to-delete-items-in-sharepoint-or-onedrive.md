---
title: Nem lehet törölni az elemeket a SharePoint vagy az OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049519"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="f063e-102">Az elemek nem törölhetők</span><span class="sxs-lookup"><span data-stu-id="f063e-102">Unable to delete items</span></span>

<span data-ttu-id="f063e-103">Problémák vannak a SharePoint-elemek törlésével?</span><span class="sxs-lookup"><span data-stu-id="f063e-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="f063e-104">Mindig győződjön meg arról, hogy rendelkezik a [megfelelő engedélyekkel](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) az elem törléséhez, vagy ha a [webhelycsoport rendszergazdája](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) megkísérli eltávolítani az elemet.</span><span class="sxs-lookup"><span data-stu-id="f063e-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="f063e-105">Ellenőrizze, hogy nincs-e az [adatmegőrzési házirend](https://docs.microsoft.com/office365/securitycompliance/retention-policies) beállítása a elemen.</span><span class="sxs-lookup"><span data-stu-id="f063e-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="f063e-106">Győződjön meg arról, hogy az elemet nem egy másik felhasználó [vette ki](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) .</span><span class="sxs-lookup"><span data-stu-id="f063e-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="f063e-107">Végül, ügyintéző tud használ [SharePoint példa és üzelmek](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) melyik tartalmaz egy könyvtár-ból PowerShell követel amit enged ön-hoz előad összetett vezetés tettek mint kényszerít törlés makacs cikk.</span><span class="sxs-lookup"><span data-stu-id="f063e-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="f063e-108">PNP-fájl eltávolítása</span><span class="sxs-lookup"><span data-stu-id="f063e-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="f063e-109">PNP-mappa eltávolítása</span><span class="sxs-lookup"><span data-stu-id="f063e-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="f063e-110">PNP-listaelem eltávolítása</span><span class="sxs-lookup"><span data-stu-id="f063e-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="f063e-111">PNP-lista eltávolítása</span><span class="sxs-lookup"><span data-stu-id="f063e-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="f063e-112">PNP mező eltávolítása (oszlop)</span><span class="sxs-lookup"><span data-stu-id="f063e-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)