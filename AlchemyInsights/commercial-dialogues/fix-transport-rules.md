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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746736"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="d7262-102">Átviteli szabályok kijavítva</span><span class="sxs-lookup"><span data-stu-id="d7262-102">Fix transport rules</span></span>

<span data-ttu-id="d7262-103">Erre az üzenetre egy egyéni e-mail-forgalom szabály vonatkozott.</span><span class="sxs-lookup"><span data-stu-id="d7262-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="d7262-104">A szabály pontos áttekintését az alábbi lépéseket kell követnie:</span><span class="sxs-lookup"><span data-stu-id="d7262-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="d7262-105">A beküldés eredményei között **a** További információk alatt jegyezze fel a **GUID azonosítót** vagy a **házirend nevét.**</span><span class="sxs-lookup"><span data-stu-id="d7262-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="d7262-106">Indítsa el az Exchange Management Shellt.</span><span class="sxs-lookup"><span data-stu-id="d7262-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="d7262-107">További információ: [Az Exchange Management Shell megnyitása.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="d7262-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="d7262-108">Futtassa ezt a parancsot (a beküldés GUID azonosítóját használva):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="d7262-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="d7262-109">A leírást áttekintve láthatja az üzenetet ható, konfigurált feltételeket.</span><span class="sxs-lookup"><span data-stu-id="d7262-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="d7262-110">További információ: [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="d7262-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
