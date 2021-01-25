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
# <a name="api-permissions-and-consent"></a>API-engedélyek és hozzájárulás

A Microsoft identitásplatformtal integrálható alkalmazások engedélyezési modellt követnek, amely lehetővé teszi a felhasználóknak és a rendszergazdáknak az adatokhoz való hozzáférés szabályozását. Az engedélyezési modell implementációja frissült a Microsoft identitásplatform végpontján. Módosítja, hogy egy alkalmazásnak hogyan kell együttműködnie a Microsoft identitásplatformtal. [A Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) identitásplatform végpontjának engedélyei és beleegyezése az engedélyezési modell alapfogalmait foglalja magában, beleértve a hatókört, az engedélyeket és a hozzájárulást.

Az [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) jóváhagyási keretrendszerével egyszerűen fejleszthet több-bérlős webes és natív ügyfélalkalmazásokat. Ezek az alkalmazások lehetővé teszik a felhasználói fiókokba való bejelentkezést egy Olyan Azure AD-bérlőből, amely eltér attól, ahol az alkalmazás regisztrálva van. A webes API-k, például a Microsoft Graph API eléréséhez (az Azure AD, az Intune és a Microsoft 365 szolgáltatásai) és más Microsoft-szolgáltatások API-jához is hozzá kell férni a saját webes API-ján kívül.

