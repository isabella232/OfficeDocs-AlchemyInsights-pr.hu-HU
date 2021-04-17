---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821449"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Az 550 5.4.1-es hibakódú továbbítási hozzáférés megtagadva kézbesítési problémáinak megoldása

Ez a [](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) probléma akkor jelentkezik, amikor ellenőrzi, hogy érvényes-e egy e-mail-cím, hogy megakadályozza a visszapattanásokat a Microsoft-hálózatba való belépéskor. Próbálkozzon az alábbiakkal:

1. Annak megállapítása, hogy a probléma egy teljes tartományra vagy egyetlen e-mail-címre jellemző-e:
    - A teljes tartomány: Időnként előfordulhat, hogy szinkronizálni kell a tartományt; próbálja [meg a tartományt Belső, majd vissza a Mérvadó beállításra.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Egyetlen e-mail-cím: Néha szinkronizálni kell a címet; az smtp-proxycím módosítása, majd visszaváltása segíthet.
2. Állapítsa meg, hogy a probléma csoportra vagy nyilvános mappára jellemző-e. Egyes objektumtípusok esetében az objektumokat manuálisan kell létrehozni az Azure Active Directoryban.

Ha további segítségre van szüksége, nyisson egy támogatási jegyet, és adja meg a probléma hatókörét (beleértve a küldeni kívánt objektum típusát), hogy jobban segítsünk Önnek.