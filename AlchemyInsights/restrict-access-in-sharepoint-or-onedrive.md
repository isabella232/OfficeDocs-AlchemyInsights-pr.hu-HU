---
title: Korlátozza a hozzáférést a SharePoint- vagy OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473431"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="eb18e-102">Korlátozza a hozzáférést a SharePoint- vagy OneDrive</span><span class="sxs-lookup"><span data-stu-id="eb18e-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="eb18e-p101">A SharePoint és a OneDrive tiltjuk meg elemekhez, például fájlok, mappák és listákat csak a csoportok vagy egyének szeretne hozzáférést nyújtó. Alapértelmezés szerint a SharePoint engedélyek hierarchiájában magasabb felfelé öröklődnek. Így a fájl az engedélyeit örökli a mappából, amelynek az engedélyeit örökli a műsortárból, amelynek az engedélyeit örökli a webhelyről.</span><span class="sxs-lookup"><span data-stu-id="eb18e-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="eb18e-p102">Megoszthatja a magasabb szintű (például egy teljes webhelyet megosztásával) és majd öröklődés megszakítása, ha nem szeretnénk megosztani a webhely elemeinek. Azonban nem ajánlott ez mert így fenntartása az engedélyeket több összetettnek és zavarosnak a jövőben. Íme, mit sikerült helyette tenni:</span><span class="sxs-lookup"><span data-stu-id="eb18e-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="eb18e-109">Ha például szeretne megosztani egy mappát, kivéve egy fájl tartalmát, helyezze át ezt a fájlt olyan helyre, amely nem osztott.</span><span class="sxs-lookup"><span data-stu-id="eb18e-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="eb18e-110">Ha egy mappában vannak almappák két, és szeretné megosztani egy almappát a és B csoportba és hozzáférést csak A csoport második almappájába, a mappa megosztása A csoport és a B csoport hozzáadása az első almappa.</span><span class="sxs-lookup"><span data-stu-id="eb18e-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="eb18e-111">Fájl vagy mappa megosztásának megszüntetése</span><span class="sxs-lookup"><span data-stu-id="eb18e-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

