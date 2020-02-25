---
title: Az Active Directory szinkronizálása nem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265198"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="5b3f2-102">Az Active Directory szinkronizálása nem</span><span class="sxs-lookup"><span data-stu-id="5b3f2-102">Active Directory not syncing</span></span>

<span data-ttu-id="5b3f2-103">Ha szinkronizálási hibákat észlel, például "nincs legutóbbi szinkronizálás", vagy észreveszi, hogy az Office felügyeleti portálon a címtár szinkronizálási állapota azt mondja: "Az utolsó szinkronizált több mint 3 nappal ezelőtt", előfordulhat, hogy az AADConnect helytelen beállításokkal rendelkezik, vagy nem elegendő engedélyeket a szinkronizálás végrehajtásához.</span><span class="sxs-lookup"><span data-stu-id="5b3f2-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="5b3f2-104">Az AADConnect expressz beállításokkal történő újratelepítése gyorsan megoldhatja a problémát:</span><span class="sxs-lookup"><span data-stu-id="5b3f2-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="5b3f2-105">[Töltse le az AADConnect legújabb verzióját.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="5b3f2-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="5b3f2-106">[Kövesse az expressz telepítésre vonatkozó utasításokat.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="5b3f2-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="5b3f2-107">Az AADConnect szolgáltatásfiókokról további információt az [Azure AD Connect: Fiókok és engedélyek](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="5b3f2-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
