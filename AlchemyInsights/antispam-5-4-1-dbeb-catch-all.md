---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717363"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>A 550 5.4.1-es hibakódok kézbesítési hibáinak elhárítása a hozzáférés megtagadásához

Ez a probléma akkor jelentkezik, ha [ellenőrzi, hogy egy e-mail-cím érvényes-e a bouncebacks megakadályozására](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) a Microsoft-hálózat beírásakor. Próbálkozzon az alábbiakkal:

1. Annak megállapítása, hogy a probléma egy teljes tartományra vagy egyetlen e-mail-címre vonatkozik-e:
    - Teljes tartomány: időnként a tartományt szinkronizálni kell; Próbálkozzon [a tartomány belső értékre állításával, majd vissza a mérvadó](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)értékre.
    - Egyetlen e-mail-cím: időnként szinkronizálni kell a címet. Ha módosítja az SMTP-proxy címét, majd újra módosítja, akkor segíthet.
2. Annak megállapítása, hogy a probléma egy csoportra vagy nyilvános mappára jellemző-e. Egyes objektumtípusok esetén előfordulhat, hogy az Azure Active Directoryban manuálisan kell létrehozni az objektumokat.

Ha további segítségre van szüksége, nyisson meg egy támogatási jegyet, és adja meg a probléma hatókörét (többek között a küldendő objektum típusát is), így jobban segíthetünk.