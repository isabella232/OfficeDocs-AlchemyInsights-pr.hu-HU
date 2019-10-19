---
title: Hozzáférés korlátozása a SharePoint vagy az OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551453"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="512ca-102">Hozzáférés korlátozása a SharePoint vagy az OneDrive</span><span class="sxs-lookup"><span data-stu-id="512ca-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="512ca-103">A SharePoint és az OneDrive alkalmazásban a fájlokhoz, mappákhoz és listákhoz hasonló elemekhez való hozzáférést úgy korlátozhatja, hogy csak az elérni kívánt csoportoknak vagy személyeknek biztosít hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="512ca-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="512ca-104">Alapértelmezés szerint a SharePoint rendszerben az engedélyek a hierarchiában feljebb lévő jogosultságoktól öröklődnek.</span><span class="sxs-lookup"><span data-stu-id="512ca-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="512ca-105">Tehát egy fájl örökli a jogosultságokat a mappából, amely örökli a jogosultságokat a könyvtár, amely örökli a jogosultságokat a hely.</span><span class="sxs-lookup"><span data-stu-id="512ca-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="512ca-106">A megosztást magasabb szinten (például egy egész webhely megosztásával) megoszthatja, majd az öröklődés megszakadhat, ha nem szeretné megosztani a webhely összes elemét.</span><span class="sxs-lookup"><span data-stu-id="512ca-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="512ca-107">Azonban ezt nem javasoljuk, mert a jogosultságokat a jövőben bonyolultabbá és bonyolultabbá teszi.</span><span class="sxs-lookup"><span data-stu-id="512ca-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="512ca-108">Itt van, mit lehetne csinálni helyette:</span><span class="sxs-lookup"><span data-stu-id="512ca-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="512ca-109">Ha például egy mappa teljes tartalmát meg szeretné osztani egy fájlon kívül, helyezze át a fájlt egy olyan új helyre, amely nincs megosztva.</span><span class="sxs-lookup"><span data-stu-id="512ca-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="512ca-110">Ha egy mappában két almappája van, és egy almappát szeretne megosztani az A és A B csoporttal, és csak az A csoport férhet hozzá a második almappához, ossza meg a szülőmappát az A csoporttal, és az első almappához vegye fel a B csoportot.</span><span class="sxs-lookup"><span data-stu-id="512ca-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="512ca-111">Fájl vagy mappa megosztásának leállítása</span><span class="sxs-lookup"><span data-stu-id="512ca-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

