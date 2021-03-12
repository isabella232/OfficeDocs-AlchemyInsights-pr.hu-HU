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
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="e9a27-102">A jelszóalapú zökkenőmentes egyszeri bejelentkezéssel kapcsolatos problémák elhárítása</span><span class="sxs-lookup"><span data-stu-id="e9a27-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="e9a27-103">A jelszóalapú SSO alapjairól az [Azure Active Directoryval való jelszóalapú hitelesítésben olvashat.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="e9a27-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="e9a27-104">**Jelszóalapú SSO konfigurálása**</span><span class="sxs-lookup"><span data-stu-id="e9a27-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="e9a27-105">[Konfigurálja a jelszóalapú egyszeri bejelentkezést](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – Ez a cikk részletesebben ismerteti a jelszóalapú egyszeri bejelentkezést.</span><span class="sxs-lookup"><span data-stu-id="e9a27-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="e9a27-106">Ha a hozzáadni szükséges alkalmazás egyéni konfigurációt igényel, és jelszóalapú SSO-t kell használnia, akkor ez a cikk Önnek készült.</span><span class="sxs-lookup"><span data-stu-id="e9a27-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="e9a27-107">[Konfigurálja a jelszóalapú egyszeri bejelentkezést a on-prem alkalmazásokhoz](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Az alkalmazásproxy számos egyszeri bejelentkezési módot támogat.</span><span class="sxs-lookup"><span data-stu-id="e9a27-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="e9a27-108">A jelszóalapú bejelentkezés olyan alkalmazásokhoz használható, amelyek hitelesítéshez felhasználónév/jelszó kombinációt használnak.</span><span class="sxs-lookup"><span data-stu-id="e9a27-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="e9a27-109">Amikor jelszóalapú bejelentkezést konfigurál az alkalmazáshoz, a felhasználóknak egyszer be kell jelentkezniük a helyszíni alkalmazásba.</span><span class="sxs-lookup"><span data-stu-id="e9a27-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="e9a27-110">Ezt követően az Azure Active Directory tárolja a bejelentkezési adatokat, és automatikusan biztosítja az alkalmazásnak, amikor a felhasználók távolról hozzáférnek.</span><span class="sxs-lookup"><span data-stu-id="e9a27-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="e9a27-111">Már közzé kellett volna tennie és tesztelnie kellett volna az alkalmazást az alkalmazásproxyval.</span><span class="sxs-lookup"><span data-stu-id="e9a27-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="e9a27-112">Ha nem, kövesse az Alkalmazások közzététele az [Azure AD alkalmazásproxyval](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) lépéseit, majd folytassa a jelszóalapú SSO konfigurációját a rendszerbeli alkalmazásokhoz.</span><span class="sxs-lookup"><span data-stu-id="e9a27-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="e9a27-113">A jelszóalapú egyszeri bejelentkezés hibaelhárításáról az [Azure AD-ban](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) a jelszóalapú egyszeri bejelentkezés hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="e9a27-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
