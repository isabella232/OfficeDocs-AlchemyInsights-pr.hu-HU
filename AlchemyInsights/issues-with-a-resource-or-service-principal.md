---
title: Problémák az erőforrásokkal vagy a szolgáltatásnévvel kapcsolatban
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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028078"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problémák az erőforrásokkal vagy a szolgáltatásnévvel kapcsolatban

1. Ha még csak most ismerkedik, az Azure Active Directory alkalmazás- és szolgáltatás-egyszerű objektumai ismertetik az [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) alkalmazásban való regisztrációt, az alkalmazásobjektumokat és a szolgáltatásnévszőket: mik azok, hogyan használják őket, és hogyan kapcsolódnak egymáshoz. Egy több-bérlős példa eset is látható az alkalmazás alkalmazásobjektuma és a kapcsolódó egyszerű szolgáltatásobjektumok közötti kapcsolat szemléltetésére.
2. Ha többet szeretne megtudni az alkalmazások és a szolgáltatásnévsok közötti kapcsolatról, olvassa el az alkalmazásokat és a szolgáltatás egyszerű [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Ennek mikéntje:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) A portál segítségével hozzon létre egy Azure AD-alkalmazást és -szolgáltatás egyszerű szolgáltatást, amely hozzáférhet az erőforrásokhoz. Ez a cikk bemutatja, hogy miként hozhat létre új Azure Active Directory (Azure AD) alkalmazást és szolgáltatásnév-egyszerű szolgáltatást, amely használható a szerepköralapú hozzáférés-vezérléssel.
4. Az egyszerű [szolgáltatás API-val](https://docs.microsoft.com/graph/api/resources/serviceprincipal)programozással kezelheti az alkalmazások példányait, és szabályozhatja, hogy egy alkalmazás mire képes a bérlői webhelyen belül.
5. [A servicePrincipal erőforrástípus](https://docs.microsoft.com/graph/api/resources/serviceprincipal) felsorolja a servicePrincipal erőforrástípus összes tulajdonságát és metódusát.
6. [Az Erőforrástípus-különbségek](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) az Azure AD-Graph és a Microsoft Graph kiemelik az Azure AD-erőforrások és a Microsoft Graph közötti Graph különbségeket. Különböző névvel vagy nem elérhető erőforrásokkal rendelkezik; a microsoftos verzió béta verziójában elérhető erőforrásokat is kiemeli Graph az 1.0-s verzióban nem.

**Problémák a vendégfelhasználóknál**

- [Rövid útmutató:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Vendégfelhasználók felvétele a címtárba az Azure Portalon bemutatja, hogy miként adhat hozzá új vendégfelhasználókat az Azure AD címtárához az Azure Portalon keresztül, hogyan küldhet meghívót, és hogyan láthatja a vendégfelhasználó meghívás-beváltási folyamatát.
- [Oktatóprogram: Felhasználói folyamatokat](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) hozhat létre a Azure Active Directory A B2C bemutatja, hogy miként hozhat létre ajánlott felhasználói folyamatokat az Azure Portal használatával. Ha az erőforrás-tulajdonosi jelszó hitelesítő adatainak (ROPC) folyamatának alkalmazásbeli beállításával kapcsolatban további információt Az erőforrás-tulajdonosi jelszó hitelesítő adatainak konfigurálása az Azure AD B2C szolgáltatásban talál.
