---
title: Vendégfelhasználói problémák elhárítása
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
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939381"
---
# <a name="troubleshoot-guest-user-issues"></a>Vendégfelhasználói problémák elhárítása

1. Az alkalmazásokhoz való vendégelérés kezeléséről a Vendég hozzáférésének kezelése [az Azure AD-hozzáférés véleményezésével.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. [Vendégfelhasználók](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)felvétele a címtárba az Azure Portalon: Ebben a rövid útmutatóban egy új vendégfelhasználót fog felvenni az Azure AD címtárába az Azure Portalon keresztül, meghívót küld, és láthatja, hogy a vendégfelhasználó meghívó-beváltási folyamata hogyan néz ki.
1. [Vendégfelhasználó hozzáadása a PowerShell használatával:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)Ebben a rövid útmutatóban a New-AzureADMSInvitation paranccsal adhat hozzá egy vendégfelhasználót az Azure-bérlőjéhez.
1. Ha meg szeretne tudni, hogy miként rendelhet hozzá felhasználókat és csoportokat a nagyvállalati alkalmazásokhoz az Azure Active Directory (Azure AD) szolgáltatásban, akár az Azure Portalról, akár a PowerShell használatával, olvassa el az Alkalmazás felhasználói hozzárendelésének kezelése a [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory (Azure AD) vállalaton keresztüli együttműködés a legtöbb, az Azure AD-val integrálható alkalmazással működik. Ebben a [cikkben](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)néhány népszerű SaaS-appnak az Azure AD B2B-val való használatra való konfigurálásához talál útmutatást.
1. Olyan szervezetként, amely az Azure Active Directory (Azure AD) vállalat B2B együttműködési képességeit használja a partnerszervezetek vendégfelhasználóinak az Azure AD-be való meghívására, mostantól hozzáférést nyújthat ezeknek a B2B-felhasználóknak a helyszíni alkalmazásokhoz. Ezek a helyszíni appok SAML-alapú hitelesítést vagy integrált Windows (IWA) használhatnak Kerberos-alapú korlátozott delegálással. További információ: Hozzáférés az [Azure AD-beli B2B-felhasználóknak a helyszíni alkalmazásokhoz.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Megtudhatja, hogyan adhat helyileg kezelt partnerfiókokat a felhőbeli erőforrásokhoz [az Azure AD vállalat b2b-alapú együttműködése segítségével.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)