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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034756"
---
# <a name="fix-transport-rules"></a>Átviteli szabályok kijavítva

Erre az üzenetre egy egyéni e-mail-forgalom szabály vonatkozott. A szabály pontos áttekintését az alábbi lépéseket kell követnie:

1. A beküldés eredményei között **a** További információk alatt jegyezze fel a **GUID azonosítót** vagy a **házirend nevét.**
2. Indítsa el Exchange Management Shellt. További információ: A Exchange [felügyeleti rendszerhéj megnyitása.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Futtassa ezt a parancsot (a beküldés GUID azonosítóját használva):  **Get-TransportRule -identity "GUID" | fl * Description***
4. A leírást áttekintve láthatja az üzenetet ható, konfigurált feltételeket.

További információ: [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
