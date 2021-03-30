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
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404871"
---
# <a name="api-permissions-and-consent-process"></a>API-engedélyek és jóváhagyási folyamat

Ahhoz, hogy az app hozzáférjen az adatokhoz a Microsoft Graph-ban, a felhasználónak vagy a rendszergazdának egy jóváhagyási folyamaton keresztül meg kell adnia számára a megfelelő engedélyeket. [A Microsoft Graph engedélyeinek referenciaa](https://docs.microsoft.com/graph/permissions-reference) felsorolja az egyes Microsoft Graph API-k főbb készletével társított engedélyeket. Útmutatást is nyújt az engedélyek használatára vonatkozóan.

**Egyszerű szolgáltatásnév beállítása vagy frissítése**

- [Serviceprincipal létrehozása](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – Ebből a cikkből azt tudhatja meg, hogy miként hozhat létre új servicePrincipal objektumot.
- Hozzon létre [egy Azure AD-appot &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) portálon – Ez a cikk bemutatja, hogy miként hozhat létre egy új Azure Active Directory -alkalmazást és szolgáltatásnév-egyszerű szolgáltatást, amely használható a szerepköralapú hozzáférés-vezérléssel.
- Alkalmazások & Azure [AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) szolgáltatásban – Ez a cikk az Azure Active Directoryban található alkalmazásregisztrációkat, alkalmazásobjektumokat és szolgáltatásnév-egyszerűket ismerteti: mik azok, hogyan használják őket, és hogyan kapcsolódnak egymáshoz.

**Alkalmazásregisztráció hozzáadása vagy frissítése, valamint rendszergazdai hozzájárulás**

- [Alkalmazásregisztráció létrehozása](https://docs.microsoft.com/graph/api/application-post-applications) – Ebből a cikkből azt tudhatja meg, hogy miként hozhat létre új alkalmazásobjektumot.
- [Alkalmazásregisztráció frissítése – API-engedélyek](https://docs.microsoft.com/graph/api/application-update) – Ebből a cikkből azt tudhatja meg, hogy miként frissítheti egy alkalmazásobjektum tulajdonságait.
- [Adja meg a rendszergazdai](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) hozzájárulást – A rendszergazdai hozzájáruláshoz és a beleegyezéshez általánosságban azt kérjük, hogy egy rendszergazda kifejezetten adja meg a hozzájárulást.
- [RBAC (béta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – Az egységes szerepkör-definíciók és szerepkör-hozzárendelések szerepkörkezelési tárolója a Microsoft 365 rbac-szolgáltatói számára, amelyek egyetlen szerepkör-hozzárendelésben támogatják a több fő tőkecsoportot és több hatókört. Ez nem különbözik *az rbacApplication* erőforrástípustól. A Microsoft Intune egy ilyen RBAC-szolgáltató példája. Az Intune-ban egy szerepkör-hozzárendelésnek lehet egy főnév-tömbje és egy hatókörcsoportok tömbje. **Ez bétaverziójú, ami azt jelenti, hogy még fejlesztés alatt áll, és nem ajánlott a fejlesztéshez.**
