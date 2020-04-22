---
title: Hozzáférés korlátozása a SharePointban vagy a OneDrive-on
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715886"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="ed3d1-102">Hozzáférés korlátozása a SharePointban vagy a OneDrive-on</span><span class="sxs-lookup"><span data-stu-id="ed3d1-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="ed3d1-103">A SharePointban és a OneDrive-ban korlátozhatja a hozzáférést az olyan elemekhez, mint a fájlok, mappák és listák, mivel csak olyan csoportoknak vagy személyeknek biztosít hozzáférést, amelyekhez hozzá szeretne férni.</span><span class="sxs-lookup"><span data-stu-id="ed3d1-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="ed3d1-104">Alapértelmezés szerint a SharePoint engedélyei a hierarchia magasabb szintű részétől öröklődnek.</span><span class="sxs-lookup"><span data-stu-id="ed3d1-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="ed3d1-105">Így egy fájl örökli az engedélyeit a mappából, amely az engedélyeket a tárból örökli, amely az engedélyeket a webhelytől örökli.</span><span class="sxs-lookup"><span data-stu-id="ed3d1-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="ed3d1-106">Magasabb szinten is megoszthatja (például egy teljes webhely megosztásával), majd megszakíthatja az öröklődést, ha nem szeretné megosztani a webhely összes elemét.</span><span class="sxs-lookup"><span data-stu-id="ed3d1-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="ed3d1-107">Ezt azonban nem javasoljuk, mert a jövőben bonyolultabbá és zavarosabbá teszi az engedélyek karbantartását.</span><span class="sxs-lookup"><span data-stu-id="ed3d1-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="ed3d1-108">Ehelyett a következőket teheti:</span><span class="sxs-lookup"><span data-stu-id="ed3d1-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="ed3d1-109">Ha például egy mappa teljes tartalmát meg szeretné osztani, kivéve egy fájlt, helyezze át a fájlt egy új helyre, amely nincs megosztva.</span><span class="sxs-lookup"><span data-stu-id="ed3d1-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="ed3d1-110">Ha egy mappában két almappa van, és egy almappát meg szeretne osztani az A és B csoporttal, és csak az A csoport számára engedélyezi a hozzáférést a második almappához, ossza meg a szülőmappát az A csoporttal, és adja hozzá a B csoportot az első almappához.</span><span class="sxs-lookup"><span data-stu-id="ed3d1-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="ed3d1-111">Fájl vagy mappa megosztásának leállítása</span><span class="sxs-lookup"><span data-stu-id="ed3d1-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

