---
title: Bérlő törlése
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993895"
---
# <a name="delete-tenant"></a>Bérlő törlése

Azure AD törléséhez győződjön meg a következő szolgáltatásokról:
- Ön a címtár globális rendszergazdája.
- NEM olyan fiókkal van bejelentkezve, amely az alapértelmezett címtárat (például contoso.onmicrosoft.com, például a admin@contoso.onmicrosoft.com.
- Törlés előtt távolítsa el az összes aktív alkalmazást a címtárból. Az aktív alkalmazások eltávolításához lépjen az Alkalmazás-regisztrációk lapra, és távolítsa el a meglévő alkalmazásokat.
- A címtárban társított Microsoft Online Szolgáltatásokhoz (például Microsoft Azure, Office 365 vagy prémium szintű Azure AD nincs aktív előfizetés. Az Előfizetések átvitele vagy az aktív előfizetések gyors lemondása az Azure Támogatási és számlázási szolgáltatáson keresztül. További információ: Az előfizetések Office 365 Azure-előfizetések lemondása. Ha segítségre van szüksége egy meglévő előfizetés bérlői fiókhoz való társításához vagy hozzáadásához, tekintse meg az Azure-előfizetés társítása vagy hozzáadása az [Azure AD-bérlőhöz lehetőséget.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Nincs aktív licenc. A licencek eltávolításáról az Előfizetés eltávolítása licenc [eltávolításához .](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Az Azure AD törlésekor nem áll más aktív felhasználó a címtárban Ön mellett globális rendszergazdaként. Távolítson el minden más aktív felhasználót, és a bérlői fiók egyéni tartománynevére vonatkozó függőségeket is el kell távolítani, például a bérlői fiókkal létrehozott admin@contoso.com.

Az alábbi lépések részletesen ismertetik az alábbi lépéseket:
- A "Azure Active Directory" vagy az "előfizetés" törléséről további [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- Alkalmazások eltávolítása a címtárból: [Alkalmazások eltávolítása.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
