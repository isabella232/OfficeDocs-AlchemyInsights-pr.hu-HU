---
title: Felhasználó létrehozása
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569732"
---
# <a name="create-user"></a>Felhasználó létrehozása

**KÖZLEMÉNY:**

- [A WebView-bejelentkezés 2021. január 4-től](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) való támogatása a Google-tól. Tesztelje, hogy az appokat érintheti-e a [Google tesztelési](https://go.microsoft.com/fwlink/?linkid=2157323) kompatibilitásra vonatkozó útmutatása.
- Mindenképpen a rendszer webböngészőt vagy a rendszernézetet használja, amikor felhasználóit fogyasztói Google-fiókokkal jelentkezik be. További információ: Problémák az alkalmazásokba való bejelentkezés során a [Chrome böngészővel.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Nem tudok új felhasználót létrehozni az Azure AD címtárban**

1. Győződjön meg arról, hogy jogosult egy új normál felhasználó létrehozására. Új normál felhasználót csak a globális rendszergazda vagy Azure Active Directory (AD) hozhat létre. Ha ön nem ezen szerepkörök valamelyikében van, kérje meg a rendszergazdát, hogy vegye fel az egyik ilyen szerepkörbe, vagy hozza létre az új felhasználói fiókot.
1. Győződjön meg arról, hogy a felhasználónév egy olyan tartományban van, amely igazolt tartományként van megtetsve az Azure AD-ban. Ha nem található ellenőrzött egyéni tartománynév az Azure AD-ban, használhatja az Azure AD kezdeti tartományát, amelynek a vége *.onmicrosoft.com.
1. Győződjön meg arról, hogy a felhasználónév olyan tartományban van, amely nincs a helyszíni AD-ről az Azure AD-hez összevontan. Nem lehet felhasználókat hozzáadni a felhőbe olyan tartománynevekkel, amelyek a helyszíni környezetből összevontak.
1. Győződjön meg arról, hogy még egyetlen másik felhasználó vagy partner sem rendelkezik az új felhasználóhoz hozzárendelni kívánt felhasználónévvel. A felhasználóneveknek egyedinek kell lennie az Azure AD-ban.
1. Lásd: [Azure AD-szerepkörök és rendszergazdák](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) az Azure AD szolgáltatáshoz.
1. Tekintse át [az](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD tartománynevét.
1. A [naplókból](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) részletesebb információkat láthat egy nemrég létrehozott vagy törölt felhasználóról, például arról, hogy ki és mikor hajtotta végre a műveletet.
1. Az új felhasználók hozzáadásáról további információt az Új felhasználó létrehozása az [Azure AD-ban](/azure/active-directory/active-directory-users-create-azure-portal)az Azure Portal használatával.
1. [Azure AD rendszergazdai szerepkörök:](/azure/active-directory/active-directory-assign-admin-roles)Rendszergazdai szerepkörengedélyek a Azure Active Directory
1. Az [Azure AD PowerShell használatával is](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)létrehozhat új felhasználót.
