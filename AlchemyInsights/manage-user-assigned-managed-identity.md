---
title: Felhasználó által hozzárendelt felügyelt identitás kezelése
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177580"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="4f2e1-102">Felhasználó által hozzárendelt felügyelt identitás kezelése</span><span class="sxs-lookup"><span data-stu-id="4f2e1-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="4f2e1-103">A felhasználó által hozzárendelt felügyelt identitás kezelése a következő tevékenységeket foglalja magában:</span><span class="sxs-lookup"><span data-stu-id="4f2e1-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="4f2e1-104">Szerepkörök hozzárendelése felhasználóhoz rendelt felügyelt identitáshoz</span><span class="sxs-lookup"><span data-stu-id="4f2e1-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="4f2e1-105">Felhasználóhoz rendelt felügyelt identitás törlése</span><span class="sxs-lookup"><span data-stu-id="4f2e1-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="4f2e1-106">Felhasználó által hozzárendelt felügyelt identitás felsorolása</span><span class="sxs-lookup"><span data-stu-id="4f2e1-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="4f2e1-107">A fent említett feladatokról az alábbi cikkekben talál további információt:</span><span class="sxs-lookup"><span data-stu-id="4f2e1-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="4f2e1-108">[Felhasználóhoz rendelt](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) felügyelt identitás létrehozása – szerepkörök hozzárendelése felhasználó által hozzárendelt felügyelt identitáshoz</span><span class="sxs-lookup"><span data-stu-id="4f2e1-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="4f2e1-109">[Felhasználóhoz](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) rendelt felügyelt identitás törlése – felhasználó által hozzárendelt felügyelt identitás törlése</span><span class="sxs-lookup"><span data-stu-id="4f2e1-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="4f2e1-110">[Felhasználóhoz rendelt](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) felügyelt identitások felsorolása – felhasználóhoz rendelt felügyelt identitások felsorolása</span><span class="sxs-lookup"><span data-stu-id="4f2e1-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="4f2e1-111">Ellenőrizze, hogy a Felügyelt **identitás** közreműködői szerepkör-hozzárendelése van-e.</span><span class="sxs-lookup"><span data-stu-id="4f2e1-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="4f2e1-112">Erre a szerepkör-hozzárendelésre a felhasználó által hozzárendelt felügyelt identitások létrehozásához és törléséhez van szükség.</span><span class="sxs-lookup"><span data-stu-id="4f2e1-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
