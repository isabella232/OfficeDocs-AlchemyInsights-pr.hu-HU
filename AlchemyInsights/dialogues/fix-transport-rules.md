---
title: Átviteli szabályok kijavítva
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694153"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="7d1c3-102">Átviteli szabályok kijavítva</span><span class="sxs-lookup"><span data-stu-id="7d1c3-102">Fix transport rules</span></span>

<span data-ttu-id="7d1c3-103">Ezt az üzenetet egy egyéni e-mail-forgalom szabálya érintette.</span><span class="sxs-lookup"><span data-stu-id="7d1c3-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="7d1c3-104">A szabály pontos áttekintését az alábbi lépéseket kell követnie:</span><span class="sxs-lookup"><span data-stu-id="7d1c3-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="7d1c3-105">A beküldés eredményei között a **További** információk alatt jegyezze fel a **GUID azonosítót** vagy **a házirend nevét.**</span><span class="sxs-lookup"><span data-stu-id="7d1c3-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="7d1c3-106">Indítsa el az Exchange Management Shellt.</span><span class="sxs-lookup"><span data-stu-id="7d1c3-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="7d1c3-107">További információ: [Az Exchange Management Shell megnyitása.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="7d1c3-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="7d1c3-108">Futtassa ezt a parancsot (a beküldés GUID azonosítóját használva):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="7d1c3-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="7d1c3-109">A leírást áttekintve láthatja az üzenetet ható, konfigurált feltételeket.</span><span class="sxs-lookup"><span data-stu-id="7d1c3-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="7d1c3-110">További információ: [Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="7d1c3-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
