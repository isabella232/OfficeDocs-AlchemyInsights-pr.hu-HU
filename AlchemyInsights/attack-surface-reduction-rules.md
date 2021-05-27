---
title: Támadásifelület-csökkentés szabályai
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676233"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="2d52e-102">Támadásifelület-csökkentés szabályai</span><span class="sxs-lookup"><span data-stu-id="2d52e-102">Attack surface reduction rules</span></span>

<span data-ttu-id="2d52e-103">A fájlok vagy mappák kizárása súlyosan csökkentheti a támadásifelület-csökkentés szabályai által nyújtott védelmet.</span><span class="sxs-lookup"><span data-stu-id="2d52e-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="2d52e-104">Azok a fájlok, amelyek futtatását egy szabály letiltotta volna, engedélyezettek, és nem rögzítettek jelentést vagy eseményt.</span><span class="sxs-lookup"><span data-stu-id="2d52e-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="2d52e-105">Kivétel minden olyan szabályra érvényes, amely engedélyezi a kivételeket.</span><span class="sxs-lookup"><span data-stu-id="2d52e-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="2d52e-106">Az ASR-kivételek ugyanazt a szintaxist használják, mint a Microsoft Defender víruskereső kizárások.</span><span class="sxs-lookup"><span data-stu-id="2d52e-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="2d52e-107">A részleteket a Kivételek beállítása és érvényesítése a Microsoft Defender víruskereső [olvassa el.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="2d52e-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="2d52e-108">A problémák elkerülése érdekében tekintse át a Kivételek definiálása során gyakran használt hibákat ismertető [ismertetőt.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="2d52e-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="2d52e-109">Nem minden asr-szabály támogatja a kivételeket.</span><span class="sxs-lookup"><span data-stu-id="2d52e-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="2d52e-110">Ha ellenőrizni tudja, hogy a szabály támogatja-e a kivételeket, tekintse meg a Támadásifelület-csökkentés szabályai [táblázatot.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="2d52e-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="2d52e-111">Támadásifelület-csökkentés szabályai</span><span class="sxs-lookup"><span data-stu-id="2d52e-111">Attack surface reduction rules</span></span>

<span data-ttu-id="2d52e-112">A szervezet támadási felülete magában foglalja az összes olyan helyet, ahol a támadóknak feltörhetik a szervezet eszközeit vagy hálózatait.</span><span class="sxs-lookup"><span data-stu-id="2d52e-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="2d52e-113">A támadási felület csökkentése azt jelenti, hogy védelmet nyújt a szervezet eszközeinek és hálózatának, így a támadóknak kevesebb módszer áll a támadásra.</span><span class="sxs-lookup"><span data-stu-id="2d52e-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="2d52e-114">A támadásifelület-csökkentés szabályainak konfigurálása segíthet a Microsoft Defender végponthoz való beállításában.</span><span class="sxs-lookup"><span data-stu-id="2d52e-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="2d52e-115">További információ:</span><span class="sxs-lookup"><span data-stu-id="2d52e-115">For more information, see:</span></span>

- [<span data-ttu-id="2d52e-116">ASR-szabály GUID-ként való leképezésének elnevezése</span><span class="sxs-lookup"><span data-stu-id="2d52e-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="2d52e-117">AsR rules requirements:</span><span class="sxs-lookup"><span data-stu-id="2d52e-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="2d52e-118">Windows 10 Pro 1709-es vagy újabb verzió</span><span class="sxs-lookup"><span data-stu-id="2d52e-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="2d52e-119">Windows 10 Enterprise 1709-es vagy újabb verzió</span><span class="sxs-lookup"><span data-stu-id="2d52e-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="2d52e-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span><span class="sxs-lookup"><span data-stu-id="2d52e-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="2d52e-121">A helyes kivétel azonosítása</span><span class="sxs-lookup"><span data-stu-id="2d52e-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="2d52e-122">Keresse meg a 1121-es vagy 1122-es eseményazonosítót a Microsoft-Windows-Windows Defender/Műveleti naplóban.</span><span class="sxs-lookup"><span data-stu-id="2d52e-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="2d52e-123">Mérje fel a blokk esetét és környezetét, és győződjön meg arról, hogy ebben az esetben fel kell oldani a blokkolást.</span><span class="sxs-lookup"><span data-stu-id="2d52e-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="2d52e-124">Olvassa el a Path (Útvonal) értéket az esemény részleteiben, amely a kivételt meghatározó érték.</span><span class="sxs-lookup"><span data-stu-id="2d52e-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="2d52e-125">A kivételt a lehető legszigorúbbra kell tenni.</span><span class="sxs-lookup"><span data-stu-id="2d52e-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="2d52e-126">Szükség esetén alkalmaz egy helyettesítő karaktereket (például Felhasználói változó cseréje).</span><span class="sxs-lookup"><span data-stu-id="2d52e-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="2d52e-127">A kivétel alkalmazása a telepítési igényeknek megfelelően.</span><span class="sxs-lookup"><span data-stu-id="2d52e-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="2d52e-128">Részletes információkért lásd: [Támadásifelület-csökkentés szabályainak testreszabása.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="2d52e-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="2d52e-129">Kivételt nem ad vissza</span><span class="sxs-lookup"><span data-stu-id="2d52e-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="2d52e-130">Állapítsa meg, hogy a szabály támogatja-e a kivételeket.</span><span class="sxs-lookup"><span data-stu-id="2d52e-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="2d52e-131">További információ: [Támadásifelület-csökkentés szabályai.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="2d52e-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="2d52e-132">Tekintse át az alkalmazott kivételeket, és ellenőrizze az elkallott vagy tévesen értelmezett helyettesítő karaktereket az esemény adataival.</span><span class="sxs-lookup"><span data-stu-id="2d52e-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="2d52e-133">További információ: Támogatott [kivételtípusok](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="2d52e-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="2d52e-134">ha a szabály túl nagy hatása van, érdemes megfontolni a szabály (vissza) naplózási módba való áthelyezését további ellenőrzéshez.</span><span class="sxs-lookup"><span data-stu-id="2d52e-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="2d52e-135">Részletes információkért lásd: [A Microsoft Defender a végpontok funkcióinak naplózási üzemmódban való használata.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="2d52e-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="2d52e-136">Támogatási adatok összegyűjtése támogatási eset megnyitásához a következő paranccsal:</span><span class="sxs-lookup"><span data-stu-id="2d52e-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="2d52e-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="2d52e-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="2d52e-138">További információért lásd: A számítógépeknek a [Microsoft Defender végpontokkal](issues-with-onboarding-machines.md)kapcsolatos problémái.</span><span class="sxs-lookup"><span data-stu-id="2d52e-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
