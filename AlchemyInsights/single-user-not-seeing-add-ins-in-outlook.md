---
title: Az egyfelhasználós bővítmények nem látnak az Outlookban
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197961"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="3f1ef-102">Az egyfelhasználós bővítmények nem látnak az Outlookban</span><span class="sxs-lookup"><span data-stu-id="3f1ef-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="3f1ef-103">Előfordulhat, hogy a felhasználó egy olyan szerepkör része, amely nem rendelkezik a megfelelő AppsForOfficeEnabled paraméterrel.</span><span class="sxs-lookup"><span data-stu-id="3f1ef-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="3f1ef-104">Futtassa ezt a parancsmaskát, és derítse ki, hogy a megfelelő szerepkör van-e társítva a felhasználóhoz:</span><span class="sxs-lookup"><span data-stu-id="3f1ef-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="3f1ef-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegálás $false | Format-Table -Automatikus szerepkör,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="3f1ef-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="3f1ef-106">További információt az [Outlook bővítményeit telepítő és kezelő rendszergazdák és felhasználók megadása](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="3f1ef-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
