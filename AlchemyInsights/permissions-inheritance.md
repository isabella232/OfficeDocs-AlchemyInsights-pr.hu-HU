---
title: Az engedélyek öröklése
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: f086bd7312772b399146cd81261f147364d64665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741953"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="21418-102">Az engedélyek öröklődésének működése a SharePointban</span><span class="sxs-lookup"><span data-stu-id="21418-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="21418-103">Alapértelmezés szerint az engedélyek a SharePointban a hierarchia magasabb szintjéről öröklődnek.</span><span class="sxs-lookup"><span data-stu-id="21418-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="21418-104">Így a fájlok öröklik az engedélyeket a mappából, amely örökli az engedélyeit a tárból, amely örökli az engedélyeit a webhelyről, amely örökli az engedélyeit a webhelycsoportban.</span><span class="sxs-lookup"><span data-stu-id="21418-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="21418-105">Az egyedi engedélyek eltávolításáról és az öröklés visszaállításáról további információt a [lista vagy tár engedélyeinek módosítása és kezelése](https://go.microsoft.com/fwlink/?linkid=869946)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="21418-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

