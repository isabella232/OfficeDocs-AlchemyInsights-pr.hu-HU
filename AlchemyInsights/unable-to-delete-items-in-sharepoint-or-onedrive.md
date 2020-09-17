---
title: Nem lehet elemeket törölni a SharePointban vagy a OneDrive-ban
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806113"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="a0a0b-102">Nem lehet elemeket törölni</span><span class="sxs-lookup"><span data-stu-id="a0a0b-102">Unable to delete items</span></span>

<span data-ttu-id="a0a0b-103">Az adatmegőrzési házirendek ezt a problémát okozhatják, le kell tiltania vagy ki kell zárnia a problémát okozó megfelelő mentességet.</span><span class="sxs-lookup"><span data-stu-id="a0a0b-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="a0a0b-104">Az adatmegőrzési házirend vagy a mentesség eltávolítása után akár 24 óra is eltelhet, amíg a módosítás érvénybe lép.</span><span class="sxs-lookup"><span data-stu-id="a0a0b-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="a0a0b-105">Ügyeljen arra, hogy az elemen ne legyen [adatmegőrzési házirend](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) -beállítás.</span><span class="sxs-lookup"><span data-stu-id="a0a0b-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="a0a0b-106">Előfordulhat, hogy a webhely túllépte a tárterület korlátozását, megnöveli a [webhely kvótáját](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) , és törli az elemet.</span><span class="sxs-lookup"><span data-stu-id="a0a0b-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="a0a0b-107">Ügyeljen arra, hogy az elem ne legyen [kivéve](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) egy másik felhasználónál.</span><span class="sxs-lookup"><span data-stu-id="a0a0b-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="a0a0b-108">Végül a rendszergazdák használhatják a [SharePoint-mintákat és-eljárásokat](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), amelyek egy PowerShell-parancsok gyűjteményét tartalmazzák, amelyek lehetővé teszik az összetett kezelési műveletek végrehajtását, például a makacs elemek törlésének kényszerítését.</span><span class="sxs-lookup"><span data-stu-id="a0a0b-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="a0a0b-109">A PNP-fájl eltávolítása</span><span class="sxs-lookup"><span data-stu-id="a0a0b-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="a0a0b-110">PNP-mappa eltávolítása</span><span class="sxs-lookup"><span data-stu-id="a0a0b-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="a0a0b-111">A PNP-listaelem eltávolítása</span><span class="sxs-lookup"><span data-stu-id="a0a0b-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="a0a0b-112">A PNP-lista eltávolítása</span><span class="sxs-lookup"><span data-stu-id="a0a0b-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="a0a0b-113">A PNP-mező (oszlop) eltávolítása</span><span class="sxs-lookup"><span data-stu-id="a0a0b-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)