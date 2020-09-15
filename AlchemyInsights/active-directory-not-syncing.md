---
title: Az Active Directory nem szinkronizálódik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697631"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="2f4ce-102">Az Active Directory nem szinkronizálódik</span><span class="sxs-lookup"><span data-stu-id="2f4ce-102">Active Directory not syncing</span></span>

<span data-ttu-id="2f4ce-103">Ha szinkronizálási hibákat kap, például "nincs legutóbbi szinkronizálás" vagy a címtár-szinkronizálási állapot megtekintése az Office felügyeleti portálon, a "legutóbbi, több mint 3 nappal korábban szinkronizált" üzenet jelenik meg, előfordulhat, hogy a AADConnect helytelen beállításokkal rendelkezik, vagy nem elegendő jogosultsága van a szinkronizálás elvégzéséhez.</span><span class="sxs-lookup"><span data-stu-id="2f4ce-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="2f4ce-104">A AADConnect újratelepítése az Express beállítások segítségével gyorsan megoldhatja a problémát:</span><span class="sxs-lookup"><span data-stu-id="2f4ce-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="2f4ce-105">[Töltse le a AADConnect legújabb verzióját](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="2f4ce-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="2f4ce-106">[Kövesse az Express telepítéssel kapcsolatos útmutatást](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="2f4ce-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="2f4ce-107">A AADConnect további információt az [Azure ad Connect: fiókok és engedélyek](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="2f4ce-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
