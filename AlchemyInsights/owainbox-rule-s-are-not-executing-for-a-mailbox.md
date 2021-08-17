---
title: 1332 OWA – A postaláda szabály(ak) nem futtathatók a postaládákban
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
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040904"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>A beérkezett üzenetek szabálya nem a várt módon működik

Ellenőrizze az alábbi beállításokat a Webes Outlook:

- Az üzeneteket a beérkezett üzenetekre vonatkozó szabályok alapján csak egyszer lehet átirányítani, átirányítani vagy megválaszolni. Egy átirányító szabály (egy levelezési szabály vagy egy átviteli szabály) legfeljebb tíz továbbítási címzettet adhat hozzá az üzenethez. További információt a Napló, az Átviteli és a Beérkezett üzenetek [szabálykorlátai című cikk tartalmaz.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- A levelezési szabályok nem működnek a másik naplópostaládán. A másodlagos naplópostafiókról további információt a Másodlagos [naplózási postaláda című cikk tartalmaz.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

A problémák megoldásához tekintse át a [Tudásbázis-cikk 2829319.](https://support.microsoft.com/kb/2829319)

Ha a korábbi problémák nem jelentkeznek, futtassa a beérkezett üzenetekre vonatkozó szabály diagnosztikai jelentését, mielőtt a problémát eszkalálja a Microsoft ügyfélszolgálatához:

1. Nyissa meg a postaládát a Webes Outlook, és kattintson a <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Gépház**  >  **Az összes Outlook Gépház**  >  **Mail**  >  **Szabályok.**

2. A lap alján kattintson a Ha a szabályok nem működnek elemre, kattintson ide **diagnosztikai jelentés létrehozásához.**
