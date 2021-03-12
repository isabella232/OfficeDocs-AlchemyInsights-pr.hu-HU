---
title: Ajánlott eljárások alkalmazása speciális keresési lekérdezésekhez
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746183"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Ajánlott eljárások alkalmazása speciális keresési lekérdezésekhez

Az alábbi ajánlott eljárásokat alkalmazva gyorsabban és elkerülheti az időtúllépéseket az összetett lekérdezések futtatásakor:

- Amikor új lekérdezéseket próbál ki, mindig korlátot használjon, hogy elkerülje a rendkívül nagy méretű találatkészletek be- vagy kiesését. Az eredményhalmaz méretének előzetes felmérésére `count` is használható.
- Először használjon időszűrőket. Ideális esetben csak hét napra korlátozza a lekérdezéseket.
- A lekérdezés elején, közvetlenül az időszűrő után vegye fel azokat a szűrőket, amelyek várhatóan eltávolítják a legtöbb adatot.
- Teljes jogkivonatok keresve a helyett `has` használja az `contains` operátort.
- Nem minden oszlopban, hanem egy adott oszlopon futtathat keresést.
- Táblázatok egyesolása esetén először adja meg azt a táblázatot, amely kevesebb sort tartalmaz.
- `project` csak a szükséges oszlopokat a összekapcsolt táblázatokból.

További információt a Speciális keresési [lekérdezési gyakorlati tanácsok .](https://go.microsoft.com/fwlink/?linkid=2144812)
