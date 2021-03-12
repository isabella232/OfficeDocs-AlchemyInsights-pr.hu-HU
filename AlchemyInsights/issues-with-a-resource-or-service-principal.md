---
title: Erőforrás- vagy szolgáltatásnévvel kapcsolatos problémák
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714076"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Erőforrás- vagy szolgáltatásnévvel kapcsolatos problémák

1. Ha még csak most ismerkedik meg, az Azure Active Directory alkalmazás- és szolgáltatása egyszerű objektumai az [Azure Active Directoryban](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) az alkalmazásregisztrációt, az alkalmazásobjektumokat és a szolgáltatásnévszőket ismertetik: mik azok, hogyan használják őket, és hogyan kapcsolódnak egymáshoz. Egy több-bérlős példa forgatókönyvet is bemutatunk, amely az alkalmazás alkalmazásobjektuma és a kapcsolódó egyszerű szolgáltatásobjektumok közötti kapcsolatot szemlélteti.
2. Az azure Active Directoryban alkalmazások és egyszerű szolgáltatásobjektumok olvasva többet is megtudhat az alkalmazások és a szolgáltatásnév közötti [kapcsolatról.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Ennek mikéntje:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) A portálon létrehozhat egy Azure AD-alkalmazást és egyszerű szolgáltatást, amely hozzáférhet az erőforrásokhoz, és bemutatja, hogy miként hozhat létre új Azure Active Directory (Azure AD) alkalmazást és egyszerű szolgáltatást, amely használható a szerepköralapú hozzáférés-vezérléssel.
4. Az egyszerű [szolgáltatás API-val](https://docs.microsoft.com/graph/api/resources/serviceprincipal)programozással kezelheti az alkalmazások példányait, és szabályozhatja, hogy egy alkalmazás mire használhatja a bérlői webhelyét.
5. [A servicePrincipal erőforrástípus](https://docs.microsoft.com/graph/api/resources/serviceprincipal) felsorolja a servicePrincipal erőforrástípus összes tulajdonságát és metódusát.
6. [Az Azure AD Graph és](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) a Microsoft Graph közötti erőforrástípus-különbségek kiemelik az Azure AD Graph és a Microsoft Graph-erőforrások közötti különbségeket. Azokat az erőforrásokat jeleníti meg, amelyek neve eltérő vagy nem érhető el; kiemeli a Microsoft Graph béta verziójában elérhető, de az 1.0-s verzióban nem elérhető erőforrásokat is.

**A vendégfelhasználók problémái**

- [Gyorsútmutató:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Vendégfelhasználók felvétele a címtárba az Azure Portalon bemutatja, hogy miként adhat hozzá új vendégfelhasználót az Azure AD címtárához az Azure Portalon keresztül, hogyan küldhet meghívót, és hogyan láthatja a vendégfelhasználó meghívó-beváltási folyamatát.
- [Oktatóprogram: Felhasználói folyamatok létrehozása az Azure Active Directory B2C-ben](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) bemutatja, hogy miként hozhat létre ajánlott felhasználói folyamatokat az Azure Portal használatával. Ha az erőforrás-tulajdonosi jelszó (ROPC) folyamatának az alkalmazásbeli beállításával kapcsolatos információkat keres, tekintse meg az erőforrás-tulajdonosi jelszó hitelesítő adatainak konfigurálása folyamatot az Azure AD B2C szolgáltatásban.
