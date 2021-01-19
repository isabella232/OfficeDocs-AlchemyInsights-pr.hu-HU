---
title: Vendégfelhasználóval kapcsolatos problémák elhárítása
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901169"
---
# <a name="troubleshoot-guest-user-issues"></a>Vendégfelhasználóval kapcsolatos problémák elhárítása

1. Az alkalmazásokhoz való vendégelérés kezeléséről a Vendég hozzáférés kezelése [az Azure AD-hozzáférés véleményezésével.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. Vendégfelhasználók felvétele a címtárba az [Azure Portalon:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)Ebben a rövid útmutatóban új vendégfelhasználót kell felvennie az Azure AD címtárába az Azure Portalon keresztül, meghívót kell küldenie, és látnia kell, hogy a vendégfelhasználó meghívó-beváltási folyamata hogyan néz ki.
1. [Vendégfelhasználó hozzáadása a PowerShell használatával:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)Ebben a rövid útmutatóban a New-AzureADMSInvitation paranccsal adhat hozzá egy vendégfelhasználót az Azure-bérlőjéhez.
1. A felhasználók és csoportok Azure Active Directory (Azure AD) nagyvállalati alkalmazásokhoz való hozzárendelésének mikéntjére vonatkozó információkért olvassa el az Azure Portalon vagy a PowerShell használatával elérhető felhasználói hozzárendelések kezelését az [Azure Active Directoryban.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Az Azure Active Directory (Azure AD) B2B együttműködés a legtöbb, az Azure AD-val integrálható alkalmazással együttműködik. Ebben a [cikkben](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)az Azure AD B2B-val használható népszerű SaaS-alkalmazások konfigurálásához talál útmutatást.
1. Olyan szervezetként, amely az Azure Active Directory (Azure AD) B2B együttműködési képességeit használja a partnerszervezetek vendégfelhasználóinak az Azure AD szolgáltatásba való meghívásához, mostantól hozzáférést nyújthat ezeknek a B2B-felhasználóknak a helyszíni alkalmazásokhoz. Ezek a helyszíni appok SAML-alapú hitelesítést vagy integrált Windows-hitelesítést (IWA) használhatnak Kerberos-kényszeres delegálással (KCD). További információt az [Azure AD-ben a B2B-felhasználók](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)hozzáférésének megadása a helyszíni alkalmazásokhoz.
1. Megtudhatja, hogy miként adhat hozzáférést a helyileg kezelt partnerfiókok számára a felhőbeli erőforrásokhoz [az Azure AD B2B együttműködésével.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)