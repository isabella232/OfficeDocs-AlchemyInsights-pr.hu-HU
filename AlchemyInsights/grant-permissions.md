---
title: Engedélyek megadása
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901183"
---
# <a name="grant-permissions"></a><span data-ttu-id="2ad11-102">Engedélyek megadása</span><span class="sxs-lookup"><span data-stu-id="2ad11-102">Grant permissions</span></span>

1. <span data-ttu-id="2ad11-103">Bérlői szintű rendszergazdai hozzájárulás [](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) **megadása:** A bérlői szintű rendszergazdai hozzájárulás megadása egy alkalmazáshoz az Azure Portalon keresztül, az Azure AD PowerShell használatával vagy a jóváhagyási kérésben való, bérlői szintű rendszergazdai hozzájárulás megadásához szükséges lépésekkel kapcsolatban.</span><span class="sxs-lookup"><span data-stu-id="2ad11-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="2ad11-104">Hozzájárulás megadása egy adott felhasználó nevében: Ahelyett, hogy **a** teljes szervezetre engedélyt adnál, a rendszergazda a [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) használatával is engedélyt adhat a delegált engedélyekhez egyetlen felhasználó nevében.</span><span class="sxs-lookup"><span data-stu-id="2ad11-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="2ad11-105">További információt a [Hozzáférés lekérte egy](https://docs.microsoft.com/graph/auth-v2-user)felhasználó nevében.</span><span class="sxs-lookup"><span data-stu-id="2ad11-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>