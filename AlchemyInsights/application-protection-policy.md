---
title: Alkalmazásvédelmi házirend
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423598"
---
# <a name="application-protection-policy"></a><span data-ttu-id="c5c4a-102">Alkalmazásvédelmi házirend</span><span class="sxs-lookup"><span data-stu-id="c5c4a-102">Application protection policy</span></span>

<span data-ttu-id="c5c4a-103">Ha most nem találja az alkalmazásvédelmi szabályzatot (APP), olvassa el az [alkalmazásvédelmi szabályzatok áttekintését.](https://docs.microsoft.com/intune/apps/app-protection-policy)</span><span class="sxs-lookup"><span data-stu-id="c5c4a-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="c5c4a-104">Az APP használatának megkezdéséhez olvassa el [Az alkalmazásvédelmi szabályzatok létrehozása és hozzárendelése című témakört.](https://docs.microsoft.com/intune/app-protection-policies)</span><span class="sxs-lookup"><span data-stu-id="c5c4a-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="c5c4a-105">Alkalmazásvédelmi házirend követelményei:</span><span class="sxs-lookup"><span data-stu-id="c5c4a-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="c5c4a-106">A felhasználó Intune- vagy EMS-licenccel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="c5c4a-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="c5c4a-107">A felhasználó az alkalmazásvédelmi házirendek által megcélzott csoporthoz tartozik.</span><span class="sxs-lookup"><span data-stu-id="c5c4a-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="c5c4a-108">Csak egy vállalati felhasználó van bejelentkezve a védett alkalmazásokba az eszközön.</span><span class="sxs-lookup"><span data-stu-id="c5c4a-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="c5c4a-109">Az alkalmazás megvalósította az [Intune SDK-t.](https://docs.microsoft.com/intune/app-sdk-get-started)</span><span class="sxs-lookup"><span data-stu-id="c5c4a-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="c5c4a-110">Az SDK-t támogató alkalmazások listáját a [Microsoft Intune által védett alkalmazások](https://docs.microsoft.com/intune/apps-supported-intune-apps)című témakörben tetszésszerint.</span><span class="sxs-lookup"><span data-stu-id="c5c4a-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="c5c4a-111">A szabályzatok azt követően érvényesek, hogy egy felhasználó, aki megfelel a fenti követelményeknek, bejelentkezik egy Intune SDK-kompatibilis alkalmazásba.</span><span class="sxs-lookup"><span data-stu-id="c5c4a-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="c5c4a-112">A házirend alkalmazásának legegyszerűbb módja, ha megkell követelni, hogy a felhasználó pin-kódot állítson be a házirendben.</span><span class="sxs-lookup"><span data-stu-id="c5c4a-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="c5c4a-113">További információ:</span><span class="sxs-lookup"><span data-stu-id="c5c4a-113">For more information, see:</span></span>

[<span data-ttu-id="c5c4a-114">APP/MAM hibaelhárítás – gyakori kérdések</span><span class="sxs-lookup"><span data-stu-id="c5c4a-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="c5c4a-115">Az alkalmazásvédelmi szabályzat beállításának ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="c5c4a-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="c5c4a-116">Az alkalmazásvédelmi szabályzat kézbesítési ütemezésének ismertetése</span><span class="sxs-lookup"><span data-stu-id="c5c4a-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="c5c4a-117">Az alkalmazásvédelmi szabályzatok figyelése</span><span class="sxs-lookup"><span data-stu-id="c5c4a-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)