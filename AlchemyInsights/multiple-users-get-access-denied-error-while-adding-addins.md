---
title: Több felhasználó is megkapja az Access Denied hibaüzenetet, miközben bővítményeket ad hozzá az Outlook ban
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423715"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="e45a4-102">Több felhasználó is megkapja az Access Denied hibaüzenetet, miközben bővítményeket ad hozzá az Outlook ban</span><span class="sxs-lookup"><span data-stu-id="e45a4-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="e45a4-103">Megadhatja, hogy a szervezet mely rendszergazdái rendelkeznek engedéllyel az Outlook bővítményeinek telepítéséhez és kezeléséhez.</span><span class="sxs-lookup"><span data-stu-id="e45a4-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="e45a4-104">Azt is megadhatja, hogy a szervezet mely felhasználói jogosultak a bővítmények saját használatra történő telepítésére és kezelésére.</span><span class="sxs-lookup"><span data-stu-id="e45a4-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="e45a4-105">További információt az [Outlook bővítményeit telepítő és kezelő rendszergazdák és felhasználók megadása](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="e45a4-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="e45a4-106">Annak ellenőrzéséhez, hogy sikeresen rendelt-e engedélyeket egy felhasználóhoz, cserélje le <Role Name> az ellenőrizendő szerepkör nevét, és futtassa a következő parancsot az Exchange Online PowerShellben:</span><span class="sxs-lookup"><span data-stu-id="e45a4-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="e45a4-107">Get-ManagementRoleAssignment -Role " <Role Name> " - GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="e45a4-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="e45a4-108">Ez a példa bemutatja, hogyan ellenőrizheti, hogy kihez rendelt engedélyeket a szervezet Office Áruházból történő telepítéséhez.</span><span class="sxs-lookup"><span data-stu-id="e45a4-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="e45a4-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="e45a4-109">PowerShell</span></span>

<span data-ttu-id="e45a4-110">-Szerep "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="e45a4-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="e45a4-111">Az eredmények, Get-ManagementRoleAssignment tekintse át a bejegyzéseket a tényleges felhasználók oszlopban.</span><span class="sxs-lookup"><span data-stu-id="e45a4-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="e45a4-112">Részletes szintaxis- és paraméterinformációkat a [Get-ManagementRoleAssignment című](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="e45a4-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 