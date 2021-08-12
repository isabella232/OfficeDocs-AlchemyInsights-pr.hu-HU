---
title: A jelszóalapú zökkenőmentes egyszeri bejelentkezéssel kapcsolatos problémák elhárítása
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
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972826"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>A jelszóalapú zökkenőmentes egyszeri bejelentkezéssel kapcsolatos problémák elhárítása

A jelszóalapú SSO alapjairól a Jelszóalapú hitelesítés jelszóval és jelszóval [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Jelszóalapú SSO konfigurálása**

1. [Jelszóalapú](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) egyszeri bejelentkezés beállítása – Ez a cikk részletesen ismerteti a jelszóalapú egyszeri bejelentkezést. Ha a hozzáadni szükséges alkalmazáshoz egyéni konfiguráció szükséges, és jelszóalapú SSO-t kell használnia, akkor ez a cikk Önnek készült.
2. Jelszóalapú egyszeri bejelentkezés beállítása a [on-prem alkalmazásokhoz](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Az alkalmazásproxy számos egyszeri bejelentkezési módot támogat. A jelszóalapú bejelentkezés olyan alkalmazásoknál használható, amelyek hitelesítéshez felhasználónév/jelszó kombinációt használnak. Amikor jelszóalapú bejelentkezést konfigurál az alkalmazáshoz, a felhasználóknak egyszer be kell jelentkezniük a helyszíni alkalmazásba. Ezt követően Azure Active Directory a bejelentkezési adatokat, és automatikusan átküldi az alkalmazásnak, amikor a felhasználók távolról hozzáférnek.
    - Már közzé kellett volna tennie és tesztelnie kellett volna az alkalmazást az Alkalmazásproxyval. Ha nem, kövesse az Alkalmazások közzététele az Azure AD-alkalmazásproxyval lépéseit, majd folytassa a jelszóalapú SSO konfigurációját a on-prem appok esetében. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)

A jelszóalapú egyszeri bejelentkezéssel kapcsolatos hibák elhárításáról A jelszóalapú egyszeri bejelentkezés hibaelhárítása az [Azure AD-ban](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
