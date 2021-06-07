---
title: Teljesítménybeli problémák a Microsoft Defender linuxos végpontja esetén
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794008"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Teljesítménybeli problémák a Microsoft Defender linuxos végpontja esetén

Ez a cikk végigvezeti a Linuxon használt Microsoft Defender végpont teljesítménybeli problémáinak azonosításához szükséges lépéseken.

Először is ellenőriznie kell, hogy a tapasztalt probléma megoldódott-e a [legújabb verzióval.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

A vizsgálat elkezdődéről A [Microsoft Defender linuxos végponttal kapcsolatos](/microsoft-365/security/defender-endpoint/linux-support-perf)teljesítményproblémák elhárítása .

## <a name="exclusions"></a>Kivételek

A kizárások segíthetnek a teljesítménybeli problémák csökkentésében. Mielőtt nekikezd, tekintse át a kivételeket, hogy minden további kockázatot ismertté és dokumentáljon.

További információ: Kivételek konfigurálása és érvényesítése a Microsoft Defenderhez a [végponthoz Linuxon.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Ha több fájlt és & kizárni, és mindegyik ugyanazon a hegyponton található, egyszerűbb lehet kizárni a rögzítőpontot. A 101.22.80-as februári kiadástól kezdve kizárhat egy teljes hegypontot.

Ha például a /mnt/backup egy hegypont, az alábbi parancs futtatásával hozzáadhatja az /mnt/backup parancsot a kizárási listához:

`$ mdatp exclusion folder add –path /mnt/backup`

**Megjegyzés:** A kizárások növelik a kártevők észlelésének kockázatát, ezért az ilyen kártevőket óvatosan kell kezelni és végrehajtani.

## <a name="need-help"></a>Segítségre van szüksége?

A támogatási eset megnyitása előtt gyűjtse össze a diagnosztikai adatokat, hogy a lehető leghatékonyabb segítséget tudja nyújtani Önnek.
