---
title: Egy felhasználó hozzáférés-megtagadási hibaüzenetet kap, miközben bővítményeket vesz fel az Outlookban
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 355f37386e0a498185e195c1d715386785d0b54b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673283"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="e752c-102">Egy felhasználó hozzáférés-megtagadási hibaüzenetet kap, miközben bővítményeket vesz fel az Outlookban</span><span class="sxs-lookup"><span data-stu-id="e752c-102">One user gets Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="e752c-103">Felhasználói PowerShell: engedélyek keresése:</span><span class="sxs-lookup"><span data-stu-id="e752c-103">User PowerShell To find permissions:</span></span>

<span data-ttu-id="e752c-104">Get-ManagementRoleAssignment-RoleAssignee [User@domain.com](mailto:user@domain.com "mailto:user@domain.com") – delegált $false | Format-Table-Auto role, RoleAssigneeName, RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="e752c-104">Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>