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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707913"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Az 550 5.4.1-es hibakódú kézbesítési problémák megoldásának megoldása megtagadva

Ez a probléma akkor fordul [elő, ha ellenőrzi, hogy érvényes-e egy e-mail cím, hogy megakadályozza a visszapattanásokat](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) a Microsoft-hálózatba való belépéskor. Próbálkozzon a következőkkel:

1. Határozza meg, hogy a probléma egy teljes tartományra vagy egyetlen e-mail címre vonatkozik-e:
    - Teljes tartomány: Néha a tartományt szinkronizálni kell; próbálja meg [a tartományt Belső, majd vissza mérvadó ra.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Egyetlen e-mail cím: Néha a címet szinkronizálni kell; megváltoztatása smtp proxy címét, majd megváltoztatja vissza segíthet.
2. Határozza meg, hogy a probléma egy csoportra vagy nyilvános mappára vonatkozik-e. Bizonyos objektumtípusok esetében előfordulhat, hogy az objektumokat manuálisan kell létrehozni az Azure Active Directoryban.

Ha további segítségre van szüksége, nyisson meg egy támogatási jegyet, és adja meg a probléma hatókörét (beleértve az elküldött objektum típusát is), hogy jobban segíthessünk Önnek.