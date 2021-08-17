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
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084096"
---
# <a name="using-dlp-in-transport-rules"></a>DLP használata az átviteli szabályokban

Az adatveszteség-megelőzés (DLP) meglévő átvitelbe való integrálásához használja a következő feltételt: „**Ha az üzenet tartalmaz... Bizalmas adatokat**“ az Átviteli szabály beállításaiban.

**További részletek:**

- Integrált DLP-bizalmasadat-típusok az átviteli szabályokban: [Bizalmas információkra vonatkozó szabályok integrálása](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Emellett a szabályt házirendteszttel vagy anélkül is tesztelheti a szabály Tesztelési módjának használatával.  Tesztelés előtt várnia kell 30 percet a szabály létrehozása után.

- Lásd: [E-mail forgalmi/Átviteli szabályok tesztelése](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

Megjegyzés: Ha egy új DLP-házirendet szeretne implementálni átviteli szabályokkal az EAC-ben, akkor ehelyett használja a [DLP-házirendeket a Biztonsági és megfelelőségi központban](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
