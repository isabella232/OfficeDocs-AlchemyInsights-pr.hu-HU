---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672435"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Fix szállítási problémák hibakódot 550 5.4.1 Relay hozzáférés megtagadva

Ez probléma előfordul mikor [korlátozás-hoz lát ha egy elektronikus levél cím van érvényes-hoz megakadályoz bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) Mikor tífusz a Hivatal 365 hálózat. Próbálkozzon a következőkkel:

1. Állapítsa meg, hogy a probléma egy teljes tartományra vagy egy e-mail címre vonatkozik-e:
    - Teljes tartomány: előfordul, hogy a tartományt szinkronizálni kell; megpróbál [elintézés a birtok-hoz belső aztán hát-hoz hiteles](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Egy e-mail cím: előfordul, hogy a címet szinkronizálni kell; megváltozó a SMTP helyettes cím aztán megváltozó ez hát tud segít.
2. Állapítsa meg, hogy a probléma egy adott csoportra vagy nyilvános mappára vonatkozik-e. Egyes objektumtípusok esetében előfordulhat, hogy a Azure Active Directory szolgáltatásban kézzel kell létrehozni az objektumokat.

Ha szüksége van további segítségre, kérjük, nyissa meg a támogatási jegyet, és adja meg a kérdés kiterjedését (includidng a típusú objektum te küldeni), hogy mi segítünk Önnek jobb.