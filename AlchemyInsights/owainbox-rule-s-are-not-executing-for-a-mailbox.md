---
title: 1332 OWA – A beérkezett üzenetek szabálya(i) nem végrehajtódnak postaládában
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576562"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>A Beérkezett üzenetek rekedése nem a várt módon működik

Ellenőrizze az alábbi beállításokat a Webes Outlookban:

- Az üzenetek csak egyszer irányíthatók át, továbbíthatók vagy válaszolhatók automatikusan a Beérkezett üzenetek szabályai alapján. Az átirányítási szabály (egy beérkezett üzenetekre vonatkozó szabály vagy levélfolyam-szabály, más néven átviteli szabály) legfeljebb tíz továbbítási címzettet adhat az üzenethez. További információt a [Napló, a Átvitel és a Beérkezett üzenetek szabálykorlátok című témakörben talál.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- A beérkezett üzenetekre vonatkozó szabályok nem működnek az alternatív naplózási postaládán. A másodlagos naplózási postaládáról további információt az [Alternatív naplózási postaláda](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)című témakörben talál.

A problémák megoldásához [lásd: KB 2829319](https://support.microsoft.com/kb/2829319).

Ha az előző problémák nem jelentkeznek, futtassa a Beérkezett üzenetek szabály diagnosztikai jelentését, mielőtt a problémát a Microsoft támogatási szolgálatra szeretné terjessni:

1. A postaláda megnyitása a Webes Outlookban, és kattintson a <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Beállítások**  >  **Az Összes Outlook-beállítás**  >  megtekintése **E-mail**  >  **Szabályok**.

2. A lap alján kattintson a **Ha a szabályok nem működnek, kattintson ide a diagnosztikai jelentés létrehozásához.**
