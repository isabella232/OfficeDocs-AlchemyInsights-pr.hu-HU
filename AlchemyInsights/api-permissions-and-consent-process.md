---
title: API-engedélyek és jóváhagyási folyamat
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
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932063"
---
# <a name="api-permissions-and-consent-process"></a>API-engedélyek és jóváhagyási folyamat

Ahhoz, hogy az app hozzáférjen az adatokhoz a Microsoft Graph-ban, a felhasználónak vagy a rendszergazdának egy jóváhagyási folyamaton keresztül meg kell adnia neki a megfelelő engedélyeket. [A Microsoft Graph az](https://docs.microsoft.com/graph/permissions-reference) engedélyekre vonatkozó referencia felsorolja a Microsoft-alkalmazások egyes fő Graph API-khoz társított engedélyeket. Útmutatást is nyújt az engedélyek használatára vonatkozóan.

**Egyszerű szolgáltatásnév beállítása vagy frissítése**

- [Serviceprincipal létrehozása](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – Ebből a cikkből azt tudhatja meg, hogy miként hozhat létre új servicePrincipal objektumot.
- [Azure AD-alkalmazás](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) & szolgáltatásnév létrehozása a portálon – Ebből a cikkből azt tudhatja meg, hogy miként hozhat létre új Azure Active Directory (Azure AD) alkalmazást és szolgáltatásnév-egyszerű szolgáltatást, amely használható a szerepköralapú hozzáférés-vezérléssel.
- [Azure](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) AD& alkalmazások – Ez a cikk az Azure Active Directory alkalmazásban való regisztrációt, az alkalmazásobjektumokat és a szolgáltatásnévszőket ismerteti: mik azok, hogyan használják őket, és hogyan kapcsolódnak egymáshoz.

**Alkalmazásregisztráció hozzáadása vagy frissítése, valamint rendszergazdai hozzájárulás**

- [Alkalmazásregisztráció létrehozása](https://docs.microsoft.com/graph/api/application-post-applications) – Ebből a cikkből azt tudhatja meg, hogy miként hozhat létre új alkalmazásobjektumot.
- [Alkalmazásregisztráció frissítése – API-engedélyek](https://docs.microsoft.com/graph/api/application-update) – Ebből a cikkből azt tudhatja meg, hogy miként frissítheti egy alkalmazásobjektum tulajdonságait.
- [Adja meg a rendszergazdai](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) hozzájárulást – A rendszergazdai hozzájáruláshoz és a beleegyezéshez általánosságban azt kérjük, hogy egy rendszergazda kifejezetten adja meg a hozzájárulást.
- [RBAC (béta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – Az egységes szerepkör-definíciók és szerepkör-hozzárendelések szerepkör-kezelési tárolója Microsoft 365 több elsődleges és több hatókört egyetlen szerepkör-hozzárendelésben támogató rbac-szolgáltatók számára. Ez nem különbözik *az rbacApplication* erőforrástípustól. Microsoft Intune egy ilyen RBAC-szolgáltató. Az Intune-ban egy szerepkör-hozzárendelésnek lehet egy főnév-tömbje és egy hatókörcsoportok tömbje. **Ez bétaverziójú, ami azt jelenti, hogy még fejlesztés alatt áll, és nem ajánlott a fejlesztéshez.**
