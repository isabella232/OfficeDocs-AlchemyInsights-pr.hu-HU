---
title: API-engedélyek és hozzájárulás
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974606"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="53607-102">API-engedélyek és hozzájárulás</span><span class="sxs-lookup"><span data-stu-id="53607-102">API permissions and consent</span></span>

<span data-ttu-id="53607-103">A Microsoft identitásplatformtal integrálható alkalmazások engedélyezési modellt követnek, amely lehetővé teszi a felhasználóknak és a rendszergazdáknak az adatokhoz való hozzáférés szabályozását.</span><span class="sxs-lookup"><span data-stu-id="53607-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="53607-104">Az engedélyezési modell implementációja frissült a Microsoft identitásplatform végpontján.</span><span class="sxs-lookup"><span data-stu-id="53607-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="53607-105">Módosítja, hogy egy alkalmazásnak hogyan kell együttműködnie a Microsoft identitásplatformtal.</span><span class="sxs-lookup"><span data-stu-id="53607-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="53607-106">[A Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) identitásplatform végpontjának engedélyei és beleegyezése az engedélyezési modell alapfogalmait foglalja magában, beleértve a hatókört, az engedélyeket és a hozzájárulást.</span><span class="sxs-lookup"><span data-stu-id="53607-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="53607-107">Az [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) jóváhagyási keretrendszerével egyszerűen fejleszthet több-bérlős webes és natív ügyfélalkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="53607-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="53607-108">Ezek az alkalmazások lehetővé teszik a felhasználói fiókokba való bejelentkezést egy Olyan Azure AD-bérlőből, amely eltér attól, ahol az alkalmazás regisztrálva van.</span><span class="sxs-lookup"><span data-stu-id="53607-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="53607-109">A webes API-k, például a Microsoft Graph API eléréséhez (az Azure AD, az Intune és a Microsoft 365 szolgáltatásai) és más Microsoft-szolgáltatások API-jához is hozzá kell férni a saját webes API-ján kívül.</span><span class="sxs-lookup"><span data-stu-id="53607-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

