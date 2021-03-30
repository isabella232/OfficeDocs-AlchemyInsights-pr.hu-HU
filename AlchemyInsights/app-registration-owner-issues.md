---
title: Alkalmazásregisztrációs tulajdonossal kapcsolatos problémák
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
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404775"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="eb8e4-102">Alkalmazásregisztrációs tulajdonossal kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="eb8e4-102">App Registration Owner issues</span></span>

<span data-ttu-id="eb8e4-103">Az appregisztrációk tulajdonosaiként az alábbi módszerek állnak rendelkezésre:</span><span class="sxs-lookup"><span data-stu-id="eb8e4-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="eb8e4-104">Az Azure AD PowerShell modul használata –</span><span class="sxs-lookup"><span data-stu-id="eb8e4-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="eb8e4-105">Referencia: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="eb8e4-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="eb8e4-106">Az Azure CLI használata – `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="eb8e4-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="eb8e4-107">Hivatkozás: [az ad app tulajdonosa](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="eb8e4-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="eb8e4-108">Az MS Graph használata –</span><span class="sxs-lookup"><span data-stu-id="eb8e4-108">Using MS Graph -</span></span>

    <span data-ttu-id="eb8e4-109">Hivatkozás: [Tulajdonos hozzáadása – Microsoft Graph 1.0-s verziójának](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="eb8e4-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="eb8e4-110">Az Azure AD portál használata – Keresse meg az portal.azure.com [>](https://portal.azure.com/) Azure Active Directory > app regisztrálása > Válassza ki az alkalmazást > Tulajdonosok > Tulajdonosok hozzáadása lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="eb8e4-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="eb8e4-111">**Nem tudja megtekinteni az alkalmazását az Alkalmazásregisztrációk panelen, még akkor sem, ha Ön az alkalmazás tulajdonosa?**</span><span class="sxs-lookup"><span data-stu-id="eb8e4-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="eb8e4-112">Az app tulajdonosa nem rendszergazdai szerepkör.</span><span class="sxs-lookup"><span data-stu-id="eb8e4-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="eb8e4-113">Ha az [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) felügyeleti portálhoz való hozzáférés korlátozása beállítás engedélyezve van, akkor csak a rendszergazda fogja tudni megtekinteni az alkalmazásokat az appregisztrációs portálon.</span><span class="sxs-lookup"><span data-stu-id="eb8e4-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="eb8e4-114">Ahhoz, hogy egy tulajdonos megtekint tudja az alkalmazásokat, tiltsa le ezt a beállítást (Állítsa ezt NEM-nek), vagy csak az adott alkalmazáshoz rendeljen rendszergazdai szerepkört a tulajdonoshoz.</span><span class="sxs-lookup"><span data-stu-id="eb8e4-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="eb8e4-115">Ehhez azonban Azure AD Premium P2 licencre lesz szüksége, és engedélyeznie kell a [Jogosultságos identitáskezelést.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="eb8e4-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
