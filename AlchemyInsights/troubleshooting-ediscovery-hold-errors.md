---
title: Hibakeresési hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676151"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="c9870-102">Hibakeresési hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="c9870-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="c9870-103">Problémákat tapasztal adiscovery-visszavételekkel kapcsolatban?</span><span class="sxs-lookup"><span data-stu-id="c9870-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="c9870-104">Íme néhány ajánlott eljárás, amit érdemes megfontolni:</span><span class="sxs-lookup"><span data-stu-id="c9870-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="c9870-105">Ellenőrizze a terjesztés állapotát.</span><span class="sxs-lookup"><span data-stu-id="c9870-105">Check the hold distribution status.</span></span>  <span data-ttu-id="c9870-106">Ha az állapot **Be (függőben)** vagy Ki **(függőben)** állapotú, várja meg, amíg befejeződik a terjesztés.</span><span class="sxs-lookup"><span data-stu-id="c9870-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="c9870-107">A frissítéseket egyetlen tömeges kérésben egyesítheti, nem kell minden tranzakcióhoz ismétlődően frissítenie a házirendet.</span><span class="sxs-lookup"><span data-stu-id="c9870-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="c9870-108">Futtassa Set-CaseHoldPolicy <policyname> -RetryDistribution parancsot a Biztonsági és megfelelőségi központ Powershellben.</span><span class="sxs-lookup"><span data-stu-id="c9870-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="c9870-109">További információt a Biztonsági [Csatlakozás PowerShell & olvashat.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="c9870-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="c9870-110">A beállítások ellenőrzéséhez szükséges lépéseket, valamint az elektronikus adatok visszavételével kapcsolatos hibák megoldását és megoldását bemutató további gyakorlati tanácsokért lásd: A elektronikus adatok visszavételével kapcsolatos [hibák elhárítása.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="c9870-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="c9870-111">Az egyéb gyakori adatfeladatokat és hibák elhárítását a Gyakori adatfelkeresési problémák felderítése, hibaelhárítása és megoldása témakörben [kaphatja meg.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="c9870-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
