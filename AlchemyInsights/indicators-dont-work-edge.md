---
title: A jelzők nem működnek az Edge böngészőben
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676243"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="f2f88-102">A jelzők nem működnek az Edge böngészőben</span><span class="sxs-lookup"><span data-stu-id="f2f88-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="f2f88-103">Miután létrehozott egy jelölőt, azt a Edge (Smartscreen) nem tudja tiszteletben hagyni.</span><span class="sxs-lookup"><span data-stu-id="f2f88-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="f2f88-104">További információ: [Jelölők létrehozása IP-hez és URL-hez/tartományhoz.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="f2f88-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="f2f88-105">1. lépés: Az alábbiak biztosítása</span><span class="sxs-lookup"><span data-stu-id="f2f88-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="f2f88-106">Ellenőrizze, hogy helyes-e a jelölő (nem írja el az IP/URL-címet, helyes művelet, a megfelelő RBAC-csoportokat).</span><span class="sxs-lookup"><span data-stu-id="f2f88-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="f2f88-107">Várjon legalább 2 órát a jelző létrehozása után, és vegye figyelembe a lehetséges késéseket.</span><span class="sxs-lookup"><span data-stu-id="f2f88-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="f2f88-108">Győződjön meg arról, hogy a rendszer(eket) a Microsoft Defenderrel való, végpontként való végre útjára vannak véve.</span><span class="sxs-lookup"><span data-stu-id="f2f88-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="f2f88-109">Ellenőrizze, hogy a rendszerek képesek-e kommunikálni a felhővel.</span><span class="sxs-lookup"><span data-stu-id="f2f88-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="f2f88-110">Ellenőrizze, hogy a Smartscreen engedélyezve van-e, és elérhető-e a [tesztwebhelyen.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="f2f88-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="f2f88-111">2. lépés: A potenciális probléma megoldása</span><span class="sxs-lookup"><span data-stu-id="f2f88-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="f2f88-112">Győződjön meg arról, hogy az ügyfél megfelel a követelményeknek.</span><span class="sxs-lookup"><span data-stu-id="f2f88-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="f2f88-113">Részletes információkért lásd: [Jelölők létrehozása IP-hez és URL-hez/tartományhoz.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="f2f88-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="f2f88-114">Győződjön meg arról, hogy az Edge böngésző legújabb verzióját használja.</span><span class="sxs-lookup"><span data-stu-id="f2f88-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="f2f88-115">A legújabb verzióra a Következő verziójú Microsoft Edge [talál.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="f2f88-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="f2f88-116">Indítsa újra a Microsoft Edge böngészőt.</span><span class="sxs-lookup"><span data-stu-id="f2f88-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="f2f88-117">Nyissa meg azt a webhelyet, amelyhez beállításjelzőt adott meg.</span><span class="sxs-lookup"><span data-stu-id="f2f88-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="f2f88-118">Ha a webhely nem a várt módon jelenik meg, folytassa a 3. lépéssel.</span><span class="sxs-lookup"><span data-stu-id="f2f88-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="f2f88-119">3. lépés: Adatgyűjtés</span><span class="sxs-lookup"><span data-stu-id="f2f88-119">Step 3: Collect data</span></span>

- <span data-ttu-id="f2f88-120">Gyűjtse **össze az MDEClientAnalyzer** diagnosztikai adatokat.</span><span class="sxs-lookup"><span data-stu-id="f2f88-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="f2f88-121">Utasításokért lásd: [A számítógépeket a Microsoft Defender végpontra való be- vagy kitöltőgépekkel kapcsolatos problémák.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="f2f88-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="f2f88-122">Ha már jól tudja telepíteni és gyűjteni a Fiddler-nyomkövetést, tekintse meg a [Telerik Fiddler (Telerik Fiddler) adatokat.](http://www.telerik.com/fiddler)</span><span class="sxs-lookup"><span data-stu-id="f2f88-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="f2f88-123">Ha a Microsoft ügyfélszolgálatának útmutatását részesíti előnyben, válassza az alábbi Támogatás ikont egy támogatási eset megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="f2f88-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
