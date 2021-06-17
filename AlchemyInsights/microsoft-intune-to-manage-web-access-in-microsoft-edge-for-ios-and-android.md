---
title: A Microsoft Intune használata a webes hozzáférés kezelésére az iOS és Android rendszerhez készült Microsoft Edge-ben
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
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989675"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="9af91-102">A Microsoft Intune használata a webes hozzáférés kezelésére az iOS és Android rendszerhez készült Microsoft Edge-ben</span><span class="sxs-lookup"><span data-stu-id="9af91-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="9af91-103">Az iOS és Android Microsoft Edge lehetővé teszi a felhasználóknak, hogy több, teljesen különálló profilból böngésszen az interneten.</span><span class="sxs-lookup"><span data-stu-id="9af91-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="9af91-104">A Microsoft 365-adatok lehető legszélesebb körű védelmi lehetőségei válnak elérhetővé, amikor előfizet az Enterprise Mobility + Security csomagra, amely tartalmazza a Microsoft Intune és az Azure Active Directory Premium funkcióit, például a feltételes hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="9af91-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="9af91-105">Legalább egy feltételes hozzáférési házirendet szeretne alkalmazni, amely (1) lehetővé teszi a felhasználóknak, hogy mobileszközökről csatlakozzanak az iOS és Android Rendszerhez készült Microsoft Edge böngészővel, és (2) védett böngészési élményt biztosító Microsoft Intune appvédelmi házirendet valósítanak meg.</span><span class="sxs-lookup"><span data-stu-id="9af91-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="9af91-106">A feltételes hozzáférés és a házirendek használatának mikéntségére vonatkozó információkért lásd:</span><span class="sxs-lookup"><span data-stu-id="9af91-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="9af91-107">Azure Active Directory feltételes hozzáférési házirendek alkalmazása</span><span class="sxs-lookup"><span data-stu-id="9af91-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="9af91-108">A Microsoft Intune appvédelmi szabályzatának létrehozása</span><span class="sxs-lookup"><span data-stu-id="9af91-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="9af91-109">Egyszeri bejelentkezés használata az Azure Active Directoryhoz csatlakoztatott webalkalmazásokban a házirend által védett böngészőkben</span><span class="sxs-lookup"><span data-stu-id="9af91-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="9af91-110">A böngészési élmény kezelése alkalmazáskonfigurációval</span><span class="sxs-lookup"><span data-stu-id="9af91-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="9af91-111">Csak munkahelyi és iskolai fiókok használatának engedélyezése</span><span class="sxs-lookup"><span data-stu-id="9af91-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="9af91-112">Általános alkalmazáskonfigurációs házirendek telepítése</span><span class="sxs-lookup"><span data-stu-id="9af91-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="9af91-113">Appkonfigurációs házirendek telepítése az adatvédelem érdekében</span><span class="sxs-lookup"><span data-stu-id="9af91-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="9af91-114">Alkalmazáskonfigurációs házirendek telepítése a Microsoft Endpoint Managerrel</span><span class="sxs-lookup"><span data-stu-id="9af91-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="9af91-115">A felügyelt alkalmazásnaplók eléréséről az [IOS](https://go.microsoft.com/fwlink/?linkid=2132578)és Android Rendszerhez készült Microsoft Edge használata felügyelt appnaplók eléréséhez .</span><span class="sxs-lookup"><span data-stu-id="9af91-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
