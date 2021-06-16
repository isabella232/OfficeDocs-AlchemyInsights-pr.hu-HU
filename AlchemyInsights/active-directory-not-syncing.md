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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930977"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="79307-102">Az Active Directory nem szinkronizál</span><span class="sxs-lookup"><span data-stu-id="79307-102">Active Directory not syncing</span></span>

<span data-ttu-id="79307-103">Ha szinkronizálási hibákat kap (például "nincs legutóbbi szinkronizálás") vagy a Office felügyeleti portálon a címtár-szinkronizálás állapotát a következőt jelenti: "Legutóbb szinkronizálva több mint 3 napja", akkor lehet, hogy az AADConnect helytelen beállításokkal rendelkezik, vagy nincs elég engedélye a szinkronizálás végrehajtásához.</span><span class="sxs-lookup"><span data-stu-id="79307-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="79307-104">Az AADConnect gyorsbeállításokkal való újratelepítése gyorsan megoldhatja a problémát:</span><span class="sxs-lookup"><span data-stu-id="79307-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="79307-105">[Töltse le az AADConnect legújabb verzióját.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="79307-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="79307-106">[Kövesse a gyors telepítés utasításait.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="79307-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="79307-107">Az Azure AD Connect szolgáltatást a Windows Server 2012 vagy újabb verziójával kell telepíteni.</span><span class="sxs-lookup"><span data-stu-id="79307-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="79307-108">A kiszolgálónak tartományhoz kell csatlakoznia, és lehet tartományvezérlő vagy tagkiszolgáló.</span><span class="sxs-lookup"><span data-stu-id="79307-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="79307-109">Az Azure AD-szolgáltatások követelményeinek és előfeltételeinek teljes Csatlakozás olvassa el Az Azure AD-szolgáltatások használatának [előfeltételei Csatlakozás.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="79307-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="79307-110">Az AADConnect szolgáltatásfiókokkal kapcsolatos további információkért lásd: [Azure AD-Csatlakozás: Fiókok és engedélyek.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="79307-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
