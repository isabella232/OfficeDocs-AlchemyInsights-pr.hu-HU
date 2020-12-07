---
title: 'RBAC szerepkörök '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583547"
---
# <a name="rbac-rules"></a><span data-ttu-id="5b467-102">RBAC szabályok</span><span class="sxs-lookup"><span data-stu-id="5b467-102">RBAC rules</span></span>

<span data-ttu-id="5b467-103">Ha az engedélyről tájékoztató hibaüzenet jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="5b467-103">If you get the permission error:</span></span> 

- <span data-ttu-id="5b467-104">**Az objektum-azonosítóval rendelkező ügyfél nem engedélyezte a hatókör feletti műveletet (kód: AuthorizationFailed)**: amikor megkísérel létrehozni egy erőforrást, ellenőrizze, hogy van-e bejelentkezve olyan felhasználóval, akinek van írási engedélye az erőforráshoz a kijelölt hatókörben.</span><span class="sxs-lookup"><span data-stu-id="5b467-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="5b467-105">Ha például egy erőforráscsoport virtuális számítógépeit szeretné kezelni, akkor a [virtuális gép közreműködői](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) szerepkört kell tartalmaznia az erőforráscsoport (vagy a szülő hatóköre) számára.</span><span class="sxs-lookup"><span data-stu-id="5b467-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="5b467-106">Az egyes beépített szerepkörök engedélyeinek listáját a [beépített szerepkörök az Azure-források esetében](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)című témakörben találhatja meg.</span><span class="sxs-lookup"><span data-stu-id="5b467-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="5b467-107">**Nincs engedélye arra, hogy támogatási kérést hozzon létre**: Ha egy támogatási jegyet próbál létrehozni vagy frissíteni, ellenőrizze, hogy jelenleg be van-e jelentkezve egy olyan felhasználóval, akinek van hozzárendelve a Microsoft. support/supportTickets/írási engedélye (például [támogatási kérelem munkatárs](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)).</span><span class="sxs-lookup"><span data-stu-id="5b467-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="5b467-108">**Nem hozhatók létre több szerepkör-hozzárendelés (kód: RoleAssignmentLimitExceeded)**: amikor megpróbál hozzárendelni egy szerepkört, próbálja meg csökkenteni a szerepkör-hozzárendelések számát úgy, hogy a szerepköröket kiosztja a csoportokba.</span><span class="sxs-lookup"><span data-stu-id="5b467-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="5b467-109">Az Azure támogatja az **2000** szerepkör-hozzárendeléseinek előfizetését.</span><span class="sxs-lookup"><span data-stu-id="5b467-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="5b467-110">Az Azure RBAC szerepköreiről további információt az [Azure RBAC szerepkörei](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="5b467-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
