---
title: DLP használata az átviteli szabályokban
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827218"
---
# <a name="using-dlp-in-transport-rules"></a>DLP használata az átviteli szabályokban

Az adatveszteség-megelőzés (DLP) meglévő átvitelbe való integrálásához használja a következő feltételt: „**Ha az üzenet tartalmaz... Bizalmas adatokat**“ az Átviteli szabály beállításaiban.

**További részletek:**

- Integrált DLP-bizalmasadat-típusok az átviteli szabályokban: [Bizalmas információkra vonatkozó szabályok integrálása](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Emellett a szabályt házirendteszttel vagy anélkül is tesztelheti a szabály Tesztelési módjának használatával.  Tesztelés előtt várnia kell 30 percet a szabály létrehozása után.

- Lásd: [E-mail forgalmi/Átviteli szabályok tesztelése](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

Megjegyzés: Ha egy új DLP-házirendet szeretne implementálni átviteli szabályokkal az EAC-ben, akkor ehelyett használja a [DLP-házirendeket a Biztonsági és megfelelőségi központban](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
