---
title: Teljesítménybeli problémák a Microsoft Defender linuxos végpontja esetén
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794008"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="4126f-102">Teljesítménybeli problémák a Microsoft Defender linuxos végpontja esetén</span><span class="sxs-lookup"><span data-stu-id="4126f-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="4126f-103">Ez a cikk végigvezeti a Linuxon használt Microsoft Defender végpont teljesítménybeli problémáinak azonosításához szükséges lépéseken.</span><span class="sxs-lookup"><span data-stu-id="4126f-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="4126f-104">Először is ellenőriznie kell, hogy a tapasztalt probléma megoldódott-e a [legújabb verzióval.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="4126f-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="4126f-105">A vizsgálat elkezdődéről A [Microsoft Defender linuxos végponttal kapcsolatos](/microsoft-365/security/defender-endpoint/linux-support-perf)teljesítményproblémák elhárítása .</span><span class="sxs-lookup"><span data-stu-id="4126f-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="4126f-106">Kivételek</span><span class="sxs-lookup"><span data-stu-id="4126f-106">Exclusions</span></span>

<span data-ttu-id="4126f-107">A kizárások segíthetnek a teljesítménybeli problémák csökkentésében.</span><span class="sxs-lookup"><span data-stu-id="4126f-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="4126f-108">Mielőtt nekikezd, tekintse át a kivételeket, hogy minden további kockázatot ismertté és dokumentáljon.</span><span class="sxs-lookup"><span data-stu-id="4126f-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="4126f-109">További információ: Kivételek konfigurálása és érvényesítése a Microsoft Defenderhez a [végponthoz Linuxon.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="4126f-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="4126f-110">Ha több fájlt és & kizárni, és mindegyik ugyanazon a hegyponton található, egyszerűbb lehet kizárni a rögzítőpontot.</span><span class="sxs-lookup"><span data-stu-id="4126f-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="4126f-111">A 101.22.80-as februári kiadástól kezdve kizárhat egy teljes hegypontot.</span><span class="sxs-lookup"><span data-stu-id="4126f-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="4126f-112">Ha például a /mnt/backup egy hegypont, az alábbi parancs futtatásával hozzáadhatja az /mnt/backup parancsot a kizárási listához:</span><span class="sxs-lookup"><span data-stu-id="4126f-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="4126f-113">**Megjegyzés:** A kizárások növelik a kártevők észlelésének kockázatát, ezért az ilyen kártevőket óvatosan kell kezelni és végrehajtani.</span><span class="sxs-lookup"><span data-stu-id="4126f-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="4126f-114">Segítségre van szüksége?</span><span class="sxs-lookup"><span data-stu-id="4126f-114">Need Help?</span></span>

<span data-ttu-id="4126f-115">A támogatási eset megnyitása előtt gyűjtse össze a diagnosztikai adatokat, hogy a lehető leghatékonyabb segítséget tudja nyújtani Önnek.</span><span class="sxs-lookup"><span data-stu-id="4126f-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
