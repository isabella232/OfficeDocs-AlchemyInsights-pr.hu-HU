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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714770"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>A jelszóalapú zökkenőmentes egyszeri bejelentkezéssel kapcsolatos problémák elhárítása

A jelszóalapú SSO alapjairól az [Azure Active Directoryval való jelszóalapú hitelesítésben olvashat.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Jelszóalapú SSO konfigurálása**

1. [Konfigurálja a jelszóalapú egyszeri bejelentkezést](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – Ez a cikk részletesebben ismerteti a jelszóalapú egyszeri bejelentkezést. Ha a hozzáadni szükséges alkalmazás egyéni konfigurációt igényel, és jelszóalapú SSO-t kell használnia, akkor ez a cikk Önnek készült.
2. [Konfigurálja a jelszóalapú egyszeri bejelentkezést a on-prem alkalmazásokhoz](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Az alkalmazásproxy számos egyszeri bejelentkezési módot támogat. A jelszóalapú bejelentkezés olyan alkalmazásokhoz használható, amelyek hitelesítéshez felhasználónév/jelszó kombinációt használnak. Amikor jelszóalapú bejelentkezést konfigurál az alkalmazáshoz, a felhasználóknak egyszer be kell jelentkezniük a helyszíni alkalmazásba. Ezt követően az Azure Active Directory tárolja a bejelentkezési adatokat, és automatikusan biztosítja az alkalmazásnak, amikor a felhasználók távolról hozzáférnek.
    - Már közzé kellett volna tennie és tesztelnie kellett volna az alkalmazást az alkalmazásproxyval. Ha nem, kövesse az Alkalmazások közzététele az [Azure AD alkalmazásproxyval](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) lépéseit, majd folytassa a jelszóalapú SSO konfigurációját a rendszerbeli alkalmazásokhoz.

A jelszóalapú egyszeri bejelentkezés hibaelhárításáról az [Azure AD-ban](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) a jelszóalapú egyszeri bejelentkezés hibaelhárítása
