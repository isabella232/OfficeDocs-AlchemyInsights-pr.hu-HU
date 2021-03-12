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
# <a name="fix-transport-rules"></a>Átviteli szabályok kijavítva

Erre az üzenetre egy egyéni e-mail-forgalom szabály vonatkozott. A szabály pontos áttekintését az alábbi lépéseket kell követnie:

1. A beküldés eredményei között **a** További információk alatt jegyezze fel a **GUID azonosítót** vagy a **házirend nevét.**
2. Indítsa el az Exchange Management Shellt. További információ: [Az Exchange Management Shell megnyitása.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Futtassa ezt a parancsot (a beküldés GUID azonosítóját használva):  **Get-TransportRule -identity "GUID" | fl * Description***
4. A leírást áttekintve láthatja az üzenetet ható, konfigurált feltételeket.

További információ: [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
