---
title: Az Active Directory nem szinkronizál
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822853"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="234b2-102">Az Active Directory nem szinkronizál</span><span class="sxs-lookup"><span data-stu-id="234b2-102">Active Directory not syncing</span></span>

<span data-ttu-id="234b2-103">Ha szinkronizálási hibákat kap (például "nincs legutóbbi szinkronizálás", vagy ha az Office felügyeleti portálján a címtár-szinkronizálás állapota a következőt jelenti: "Utolsó szinkronizálás több mint 3 napja", akkor lehet, hogy az AADConnect helytelen beállításokkal rendelkezik, vagy nincs elég engedélye a szinkronizálás végrehajtásához.</span><span class="sxs-lookup"><span data-stu-id="234b2-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="234b2-104">Az AADConnect gyorsbeállításokkal való újratelepítése gyorsan megoldhatja a problémát:</span><span class="sxs-lookup"><span data-stu-id="234b2-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="234b2-105">[Töltse le az AADConnect legújabb verzióját.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="234b2-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="234b2-106">[Kövesse a gyors telepítés utasításait.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="234b2-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="234b2-107">Az AADConnect szolgáltatásfiókokkal kapcsolatos további információkért lásd: [Azure AD Connect: Fiókok és engedélyek.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="234b2-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
