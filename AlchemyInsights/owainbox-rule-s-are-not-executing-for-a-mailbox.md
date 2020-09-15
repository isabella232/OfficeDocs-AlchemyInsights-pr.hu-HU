---
title: Az 1332 OWA-beérkezett üzenetekre vonatkozó szabály (ok) nem egy postaládában van végrehajtva
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721593"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>A beérkezett üzenetekre vonatkozó szabályok nem a várt módon működnek

Ellenőrizze a következő beállításokat a webes Outlookban:

- Egy üzenet átirányítása, továbbítása vagy megválaszolása automatikusan a Beérkezett üzenetek szabályaitól függően csak egyszer történik meg. Egy átirányítási szabály (egy levelezési szabály vagy egy e-mail-forgalom szabálya, más néven átviteli szabály) legfeljebb tíz továbbítási címzettet adhat az üzenethez. További információ: a [Journal, a Transport és a beérkezett üzenetekre vonatkozó szabályok korlátai](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- A beérkezett üzenetekre vonatkozó szabályok nem működnek a másodlagos naplózási postaládában. A másodlagos naplózási postaládáról a [másodlagos naplózási postaláda](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)című témakörben olvashat bővebben.

A fenti problémák megoldásához lásd: [KB 2829319](https://support.microsoft.com/kb/2829319).

Ha a korábbi problémák nem érvényesek, futtassa a Beérkezett üzenetek szabály diagnosztikai jelentését, mielőtt a problémát a Microsoft támogatási szolgálata előtt kiterjesztheti:

1. Nyissa meg a postaládát a webes Outlookban, és kattintson a <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Settings (beállítások**  >  ) **Az Outlook összes beállításának megtekintése**  >  **Posta (posta**  >  ) **Szabályok**.

2. A lap alján kattintson a **Ha a szabályok nem megfelelőek, kattintson ide a diagnosztikai jelentés létrehozásához**.
