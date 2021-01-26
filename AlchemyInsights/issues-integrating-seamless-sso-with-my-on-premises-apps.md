---
title: Problémák a zökkenőmentes egyszeri bejelentkezés integrálásával a helyszíni appokkal
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868715"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="5db93-102">Problémák a zökkenőmentes egyszeri bejelentkezés integrálásával a helyszíni appokkal</span><span class="sxs-lookup"><span data-stu-id="5db93-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="5db93-103">A zökkenőmentes egyszeri bejelentkezés helyszíni alkalmazásokkal való integrálásával kapcsolatos hibák elhárításához tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="5db93-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="5db93-104">**Ajánlott lépések**</span><span class="sxs-lookup"><span data-stu-id="5db93-104">**Recommended steps**</span></span>

1. <span data-ttu-id="5db93-105">Ha egy **helyszíni alkalmazást konfigurálni** az alkalmazásproxyn keresztüli egyszeri bejelentkezéshez, tekintse meg az alkalmazásproxyval történő egyszeri bejelentkezéshez szükséges [jelszó-tárolót.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)</span><span class="sxs-lookup"><span data-stu-id="5db93-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="5db93-106">**Alkalmazásproxyval** kapcsolatos hibák elhárítása: Azt javasoljuk, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)hogy a hibakeresési folyamat, az alkalmazásproxy-összekötő hibáinak áttekintésével kezdje annak megállapítását, hogy az alkalmazásproxy-összekötők megfelelően vannak-e konfigurálva.</span><span class="sxs-lookup"><span data-stu-id="5db93-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="5db93-107">Ha továbbra is problémákat okoz az alkalmazáshoz való kapcsolódás, kövesse a hibakeresési alkalmazásproxyval kapcsolatos problémák hibaelhárítási [lépéseit.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)</span><span class="sxs-lookup"><span data-stu-id="5db93-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="5db93-108">A [CORS-problémákat az](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) alábbi böngésző hibakeresési eszközökkel azonosíthatja:</span><span class="sxs-lookup"><span data-stu-id="5db93-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="5db93-109">Indítsa el a böngészőt, és keresse meg a webalkalmazást.</span><span class="sxs-lookup"><span data-stu-id="5db93-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="5db93-110">Nyomja le **az F12 billentyűt** a hibakeresési konzolhoz való bekapcsoláshoz.</span><span class="sxs-lookup"><span data-stu-id="5db93-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="5db93-111">Próbálja meg reprodukálni a tranzakciót, és tekintse át a konzolüzenetet.</span><span class="sxs-lookup"><span data-stu-id="5db93-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="5db93-112">A CORS-szabálysértés konzolhiba esetén a forrással kapcsolatos hibát jelez.</span><span class="sxs-lookup"><span data-stu-id="5db93-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="5db93-113">Egyes CORS-problémákat nem lehet megoldani, például amikor az app átirányítja a login.microsoftonline.com hitelesítéshez, és a hozzáférési jogkivonat lejár.</span><span class="sxs-lookup"><span data-stu-id="5db93-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="5db93-114">A CORS-hívás ezután meghiúsul.</span><span class="sxs-lookup"><span data-stu-id="5db93-114">The CORS call then fails.</span></span> <span data-ttu-id="5db93-115">Kerülő megoldásként meghosszabbíthatja a hozzáférési jogkivonat teljes élettartamát, hogy megakadályozza, hogy lejár a felhasználó munkamenete során.</span><span class="sxs-lookup"><span data-stu-id="5db93-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="5db93-116">Ennek mikéntjeről a Konfigurálható jogkivonat-élettartamok a [Microsoft identitásplatformján olvashatók.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="5db93-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="5db93-117">**Ajánlott dokumentumok**</span><span class="sxs-lookup"><span data-stu-id="5db93-117">**Recommended documents**</span></span>

- [<span data-ttu-id="5db93-118">Egyszeri bejelentkezés beállítása alkalmazásproxy-alkalmazáshoz</span><span class="sxs-lookup"><span data-stu-id="5db93-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="5db93-119">SAML egyszeri bejelentkezés helyszíni alkalmazásokhoz alkalmazásproxyval</span><span class="sxs-lookup"><span data-stu-id="5db93-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="5db93-120">Az Azure Active Directory alkalmazásproxy CORS-problémáinak megoldása és használata</span><span class="sxs-lookup"><span data-stu-id="5db93-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="5db93-121">A Kerberos kényszeres delegálás konfigurálásával kapcsolatos hibák elhárítása alkalmazásproxy esetén</span><span class="sxs-lookup"><span data-stu-id="5db93-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)