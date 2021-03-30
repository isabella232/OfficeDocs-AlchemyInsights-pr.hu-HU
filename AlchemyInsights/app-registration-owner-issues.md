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
# <a name="app-registration-owner-issues"></a>Alkalmazásregisztrációs tulajdonossal kapcsolatos problémák

Az appregisztrációk tulajdonosaiként az alábbi módszerek állnak rendelkezésre:

- Az Azure AD PowerShell modul használata –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referencia: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Az Azure CLI használata – `az ad app owner add`

    Hivatkozás: [az ad app tulajdonosa](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Az MS Graph használata –

    Hivatkozás: [Tulajdonos hozzáadása – Microsoft Graph 1.0-s verziójának](https://docs.microsoft.com/graph/api/application-post-owners)
- Az Azure AD portál használata – Keresse meg az portal.azure.com [>](https://portal.azure.com/) Azure Active Directory > app regisztrálása > Válassza ki az alkalmazást > Tulajdonosok > Tulajdonosok hozzáadása lehetőséget.

**Nem tudja megtekinteni az alkalmazását az Alkalmazásregisztrációk panelen, még akkor sem, ha Ön az alkalmazás tulajdonosa?**

Az app tulajdonosa nem rendszergazdai szerepkör. Ha az [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) felügyeleti portálhoz való hozzáférés korlátozása beállítás engedélyezve van, akkor csak a rendszergazda fogja tudni megtekinteni az alkalmazásokat az appregisztrációs portálon. Ahhoz, hogy egy tulajdonos megtekint tudja az alkalmazásokat, tiltsa le ezt a beállítást (Állítsa ezt NEM-nek), vagy csak az adott alkalmazáshoz rendeljen rendszergazdai szerepkört a tulajdonoshoz. Ehhez azonban Azure AD Premium P2 licencre lesz szüksége, és engedélyeznie kell a [Jogosultságos identitáskezelést.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
