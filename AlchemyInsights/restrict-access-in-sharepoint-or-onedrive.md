---
title: Hozzáférés korlátozása a SharePointban vagy a OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720684"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="e4dc1-102">Hozzáférés korlátozása a SharePointban vagy a OneDrive</span><span class="sxs-lookup"><span data-stu-id="e4dc1-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="e4dc1-103">A SharePointban és a OneDrive a hozzáférést csak olyan csoportoknak vagy magánszemélyeknek engedélyezi, akiknek hozzáférése van.</span><span class="sxs-lookup"><span data-stu-id="e4dc1-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="e4dc1-104">Alapértelmezés szerint az engedélyek a SharePointban a hierarchia magasabb szintjéről öröklődnek.</span><span class="sxs-lookup"><span data-stu-id="e4dc1-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="e4dc1-105">Így a fájlok öröklik az engedélyeket a mappából, amely örökli az engedélyeit a tárból, ami örökli az engedélyeit a webhelyről.</span><span class="sxs-lookup"><span data-stu-id="e4dc1-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="e4dc1-106">Megoszthat magasabb szintre (például egy teljes webhely megosztásával), majd megszakíthatja az öröklést, ha nem szeretné megosztani a webhely összes elemét.</span><span class="sxs-lookup"><span data-stu-id="e4dc1-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="e4dc1-107">Ezt azonban nem javasoljuk, mert az engedélyeket a jövőben összetettebbvé és zavarosnak tartja.</span><span class="sxs-lookup"><span data-stu-id="e4dc1-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="e4dc1-108">Az alábbi műveleteket végezheti el:</span><span class="sxs-lookup"><span data-stu-id="e4dc1-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="e4dc1-109">Ha például egy mappa teljes tartalmát szeretné megosztani, kivéve az egyik fájlt, helyezze át a fájlt egy olyan új helyre, amely nincs megosztva.</span><span class="sxs-lookup"><span data-stu-id="e4dc1-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="e4dc1-110">Ha egy mappában két almappája van, és egy almappát szeretne megosztani az A és A B csoporttal, és csak a második almappához szeretne hozzáférést engedélyezni, ossza meg a szülőmappa az A és b csoporttal, és vegye fel a B csoportot az első almappába.</span><span class="sxs-lookup"><span data-stu-id="e4dc1-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="e4dc1-111">Fájl vagy mappa megosztásának megszüntetése </span><span class="sxs-lookup"><span data-stu-id="e4dc1-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

