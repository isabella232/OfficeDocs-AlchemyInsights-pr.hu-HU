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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932099"
---
# <a name="api-permissions-and-consent"></a>API-engedélyek és hozzájárulás

Az adatokkal integrálható Microsoft Identitásplatform engedélyezési modell alapján a felhasználók és a rendszergazdák szabályozhatják az adatokhoz való hozzáférést. Az engedélyezési modell implementációja frissült a Microsoft Identitásplatform végponton. Módosítja, hogy egy alkalmazásnak hogyan kell együttműködnie a Microsoft Identitásplatform. [A végpont engedélyeinek](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) és beleegyezésének Microsoft Identitásplatform az engedélyezési modell alapfogalmairól, többek között a hatókörökről, az engedélyekről és a hozzájárulásról.

A [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) jóváhagyási keretrendszer egyszerűvé teszi a több-bérlős webes és natív ügyfélalkalmazások fejlesztése. Ezek az alkalmazások lehetővé teszik a felhasználói fiókokba való bejelentkezést egy Azure AD bérlői fiókból, amely eltér attól, ahol az alkalmazás regisztrálva van. Emellett szükség lehet a webes API-k, például a Microsoft Graph API elérésére (az Azure AD, az Intune és a szolgáltatások eléréséhez az Microsoft 365-ban) és más Microsoft-szolgáltatások API-khoz is, valamint a saját webes API-khoz.

