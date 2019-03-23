---
title: Engedélyek öröklődése
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 8/7/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 5a72a74710a01cf958fa468b80ee67a4034c4383
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30752204"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="1118b-102">Engedélyek öröklése a SharePoint működése</span><span class="sxs-lookup"><span data-stu-id="1118b-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="1118b-103">Alapértelmezés szerint a SharePoint engedélyek hierarchiájában magasabb felfelé öröklődnek.</span><span class="sxs-lookup"><span data-stu-id="1118b-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="1118b-104">Így a fájl az engedélyeit örökli a mappából, amelynek az engedélyeit örökli az engedélyeit örökli annak engedélyeit örökli a webhelycsoport webhelyről származó könyvtárában lévő.</span><span class="sxs-lookup"><span data-stu-id="1118b-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="1118b-105">Egyedi engedélyek eltávolítása, és az öröklődés visszaállításával kapcsolatos információ [Szerkesztés, és a lista vagy tár engedélyeinek kezelése](https://go.microsoft.com/fwlink/?linkid=869946)témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="1118b-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

