---
title: Bejelentkezési problémák
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901018"
---
# <a name="sign-out-issues"></a><span data-ttu-id="6a2c7-102">Bejelentkezési problémák</span><span class="sxs-lookup"><span data-stu-id="6a2c7-102">Sign-out issues</span></span>

<span data-ttu-id="6a2c7-103">A kijelentkezve kapcsolatos problémák megoldásához végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="6a2c7-103">To resolve issues related to signing out, perform the following steps:</span></span>

1. <span data-ttu-id="6a2c7-104">Ha Ön vagy egy felhasználó naplózott vagy ki van jelentkezve [](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) az alkalmazásokból, kövesse a hitelesítési munkamenetek kezelésének konfigurálása feltételes hozzáféréssel vagy konfigurálható jogkivonat-élettartamokkal a [Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)identitásplatformján.</span><span class="sxs-lookup"><span data-stu-id="6a2c7-104">If you or a user are getting logged or kicked out of applications, follow the guidance in the articles [Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) or [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="6a2c7-105">A legtöbb egyéb bejelentkezési hiba vagy probléma megoldható az Azure Active Directory (Azure AD) adott alkalmazással való integrálásával.</span><span class="sxs-lookup"><span data-stu-id="6a2c7-105">Most other sign-out errors or problems can be solved by troubleshooting the integration of Azure Active Directory (Azure AD) with the specific application.</span></span> <span data-ttu-id="6a2c7-106">Adott integrációhoz útmutatást találhat az Azure [Active Directoryval](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)integráló alkalmazásokhoz használható oktatóanyagok gyűjteményében, beleértve az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="6a2c7-106">You can find guidance for a specific integration by going to this [collection of tutorials for integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), including:</span></span>
    - <span data-ttu-id="6a2c7-107">SaaS-alkalmazások oktatóanyagai</span><span class="sxs-lookup"><span data-stu-id="6a2c7-107">SaaS application tutorials</span></span>
    - <span data-ttu-id="6a2c7-108">Egyszeri bejelentkezést ismertető oktatóanyagok</span><span class="sxs-lookup"><span data-stu-id="6a2c7-108">Single sign-on tutorials</span></span>
    - <span data-ttu-id="6a2c7-109">Felhasználói kiépítési oktatóanyagok</span><span class="sxs-lookup"><span data-stu-id="6a2c7-109">User-provisioning tutorials</span></span>