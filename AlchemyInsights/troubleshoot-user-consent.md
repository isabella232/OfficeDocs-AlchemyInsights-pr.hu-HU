---
title: Felhasználó beleegyezésével kapcsolatos hibák elhárítása
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
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901190"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="ca31e-102">Felhasználó beleegyezésével kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="ca31e-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="ca31e-103">Beállíthatja, hogy a végfelhasználók hogyan járulnak hozzá az alkalmazásokhoz az Azure Portalon vagy a PowerShellen keresztül.</span><span class="sxs-lookup"><span data-stu-id="ca31e-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="ca31e-104">További [információért tekintse](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) meg a felhasználói hozzájárulási beállításokat.</span><span class="sxs-lookup"><span data-stu-id="ca31e-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="ca31e-105">A rendszergazdák a [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) használatával is engedélyt adhatnak a delegált engedélyekhez egyetlen felhasználó nevében.</span><span class="sxs-lookup"><span data-stu-id="ca31e-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="ca31e-106">További információt a [Hozzáférés lekérte egy](https://docs.microsoft.com/graph/auth-v2-user)felhasználó nevében.</span><span class="sxs-lookup"><span data-stu-id="ca31e-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="ca31e-107">[Felhasználói jóváhagyási hibák:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)Ez a cikk az alkalmazásokhoz való beleegyezés során előforduló hibákat ismerteti.</span><span class="sxs-lookup"><span data-stu-id="ca31e-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="ca31e-108">Ha hibaüzenetet nem tartalmazó váratlan jóváhagyási kéréseket hárít el, tekintse át az Azure AD hitelesítési [forgatókönyveit.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="ca31e-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>