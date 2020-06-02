---
title: Nem lehet törölni az elemeket a SharePointban vagy a OneDrive-on
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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511978"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="71989-102">Nem lehet törölni az elemeket</span><span class="sxs-lookup"><span data-stu-id="71989-102">Unable to delete items</span></span>

<span data-ttu-id="71989-103">Az adatmegőrzési házirendek ezt okozhatják, le kell tiltania vagy ki kell zárnia a problémát okozó megfelelő visszatartást.</span><span class="sxs-lookup"><span data-stu-id="71989-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="71989-104">Az adatmegőrzési szabály vagy a visszatartás eltávolítása után akár 24 órát is igénybe vehet, amíg a módosítás érvénybe lép.</span><span class="sxs-lookup"><span data-stu-id="71989-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="71989-105">Győződjön meg arról, hogy nincs [adatmegőrzési házirend](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) beállítása a cikken.</span><span class="sxs-lookup"><span data-stu-id="71989-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="71989-106">Előfordulhat, hogy a hely túllépte a tárolási korlátot, növelheti a [helykvótát,](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) és törölheti az elemet.</span><span class="sxs-lookup"><span data-stu-id="71989-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="71989-107">Győződjön meg arról, hogy az elemet nem [vette ki](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) egy másik felhasználónak.</span><span class="sxs-lookup"><span data-stu-id="71989-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="71989-108">Végül a rendszergazdák [használhatják a SharePoint Minták és gyakorlatok](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), amely egy könyvtár a PowerShell-parancsok, amelyek lehetővé teszik, hogy összetett felügyeleti műveletek, például a makacs elemek kényszerítése.</span><span class="sxs-lookup"><span data-stu-id="71989-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="71989-109">PNP-fájl eltávolítása</span><span class="sxs-lookup"><span data-stu-id="71989-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="71989-110">PNP-mappa eltávolítása</span><span class="sxs-lookup"><span data-stu-id="71989-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="71989-111">PNP-listaelem eltávolítása</span><span class="sxs-lookup"><span data-stu-id="71989-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="71989-112">PNP-lista eltávolítása</span><span class="sxs-lookup"><span data-stu-id="71989-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="71989-113">PNP-mező eltávolítása (oszlop)</span><span class="sxs-lookup"><span data-stu-id="71989-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)