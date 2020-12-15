---
title: A Microsoft Intune használata a webes hozzáférés kezeléséhez az iOS és az Android rendszerhez készült Microsoft Edge-ben
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
- "9003846"
- "6895"
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/10/2020
ms.locfileid: "49678258"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="175c9-102">A Microsoft Intune használata a webes hozzáférés kezeléséhez az iOS és az Android rendszerhez készült Microsoft Edge-ben</span><span class="sxs-lookup"><span data-stu-id="175c9-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="175c9-103">Az iOS és az Android rendszerhez készült Microsoft Edge segítségével a felhasználók több, teljesen különálló profilból tallózhatnak a weben.</span><span class="sxs-lookup"><span data-stu-id="175c9-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="175c9-104">A Microsoft 365-es adatszolgáltatások széles körű védelmi lehetőségei elérhetővé válnak a nagyvállalati Mobility + biztonsági csomagra való feliratkozáskor, beleértve a Microsoft Intune és az Azure Active Directory prémium funkciókat, például a feltételes hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="175c9-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="175c9-105">Minimálisan telepítenie kell egy feltételes hozzáférési házirendet, amely (1) lehetővé teszi, hogy a felhasználók az iOS és az Android rendszerhez az iOS és az Android rendszerhez csatlakozhassanak a Microsoft Edge-hez, és hogy (2) implementálja a védett böngészési lehetőségeket biztosító Microsoft Intune alkalmazás-védelmi házirendet.</span><span class="sxs-lookup"><span data-stu-id="175c9-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="175c9-106">Ha meg szeretné tudni, hogy miként használhatja a feltételes hozzáférést és a házirendeket, olvassa el a következő témaköröket:</span><span class="sxs-lookup"><span data-stu-id="175c9-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="175c9-107">Az Azure Active Directory feltételes elérési házirendjének alkalmazása</span><span class="sxs-lookup"><span data-stu-id="175c9-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="175c9-108">A Microsoft Intune app védelmi házirendjeinek létrehozása</span><span class="sxs-lookup"><span data-stu-id="175c9-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="175c9-109">Egyszeri bejelentkezés használata az Azure Active Directory szolgáltatáshoz – kapcsolódó webalkalmazások a házirendekkel védett böngészőkben</span><span class="sxs-lookup"><span data-stu-id="175c9-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="175c9-110">Az App-konfiguráció használata a böngészési élmény kezeléséhez</span><span class="sxs-lookup"><span data-stu-id="175c9-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="175c9-111">Kizárólag munkahelyi és iskolai fiókok használatának engedélyezése</span><span class="sxs-lookup"><span data-stu-id="175c9-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="175c9-112">Általános alkalmazás-beállítási házirendek telepítése</span><span class="sxs-lookup"><span data-stu-id="175c9-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="175c9-113">Az App konfigurációs házirendjeinek központi telepítése az adatvédelem céljából</span><span class="sxs-lookup"><span data-stu-id="175c9-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="175c9-114">Az alkalmazások konfigurálására szolgáló házirendek központi telepítése a Microsoft Endpoint Manager segítségével</span><span class="sxs-lookup"><span data-stu-id="175c9-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="175c9-115">Ha meg szeretné tudni, hogy miként férhet hozzá a felügyelt app-naplókhoz, olvassa el a [felügyelt app-naplók elérése a Microsoft Edge for iOS és az Android](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="175c9-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
