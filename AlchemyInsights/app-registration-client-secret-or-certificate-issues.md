---
title: Alkalmazásregisztrációs ügyfélprogram titkos vagy tanúsítványokkal kapcsolatos problémák
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404786"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="7e8c6-102">Alkalmazásregisztrációs ügyfélprogram titkos vagy tanúsítványokkal kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="7e8c6-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="7e8c6-103">Application client secret expiring? (Az alkalmazás titkos titkos lejárata)</span><span class="sxs-lookup"><span data-stu-id="7e8c6-103">Application client secret expiring?</span></span>

<span data-ttu-id="7e8c6-104">Függetlenül attól, hogy hogyan jött létre a regisztrált alkalmazás, akár az alkalmazások regisztrációs portáljának szokásos regisztrációs folyamatával, akár a szolgáltatásnév az alkalmazás-jóváhagyással jött létre a bérlői webhelyen, a jelenlegi kód lejárata előtt új ügyfélkódot kell létrehozni, és frissíteni kell a kapcsolódó alkalmazáskódban.</span><span class="sxs-lookup"><span data-stu-id="7e8c6-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="7e8c6-105">A maximális érvényességi idő 2 év.</span><span class="sxs-lookup"><span data-stu-id="7e8c6-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="7e8c6-106">Emlékeztetőként a titkos értéket rögzíteni kell, mivel az nem lesz látható, miután kilép az App-regisztrációk lapról a portálon.</span><span class="sxs-lookup"><span data-stu-id="7e8c6-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="7e8c6-107">További információ: Rövid útmutató: Alkalmazás regisztrálása [a Microsoft identitásplatformján](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) és Ajánlott [eljárások a Microsoft-identitásplatformhoz.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="7e8c6-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="7e8c6-108">További információ: [Azure AD-app & szolgáltatásnév a portálon – Microsoft-identitásplatform.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="7e8c6-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
