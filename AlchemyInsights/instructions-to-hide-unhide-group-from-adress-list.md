---
title: Utasítások a csoport elrejtésére/felfedésére a címlistából
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908346"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="e3c89-102">A Microsoft 365-csoport elrejtése a címlistából (GAL)</span><span class="sxs-lookup"><span data-stu-id="e3c89-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="e3c89-103">Ha egy Microsoft 365-ös csoportot el szeretne rejteni az Exchange-ügyfelek (például az Outlook vagy az OWA) címlistáiból, használja a következő parancsot az EXO rendszerhéjban:</span><span class="sxs-lookup"><span data-stu-id="e3c89-103">To hide an Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="e3c89-104">Ha el szeretné rejteni, hogy a Microsoft 365 csoport nem lesz látható az Exchange-ügyfelek számára, használja a következő parancsot az EXO rendszerhéjban:</span><span class="sxs-lookup"><span data-stu-id="e3c89-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

