---
title: 'Hiba: A számítógépen lévő szabályok nem egyeznek'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664248"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Hiba: A számítógépen lévő szabályok nem egyeznek

Az ismert probléma frissített állapotának megtekintéséhez olvassa el [A számítógépen lévő szabályok nem egyeznek meg a Microsoft Exchange szabályaival.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Az Outlook Csapat megvalósított egy javítást az 12928.10000 buildben. A javítás már az Insider Fast-nál van, és 2020 júniusának végén a Monthly Channel-re kerül. Miután a fix épít lehet, hogy a gyors "Milyen szabályokat akarsz tartani" még egyszer utoljára. Ha a rendszer kéri, válassza a Kiszolgáló lehetőséget, majd lépjen vissza az Outlook programban, és engedélyezze újra a letiltott szabályokat.

Amíg a javítás elérhetővé nem válik, használja a következő kerülő megoldást:

**Megoldás:** A legutóbbi jelentésekben a probléma azok esetében fordult elő, akik csak ügyfélszabályokat hoztak létre az Outlook asztalon. Ha továbbra is problémákkal küzd, fontolja meg a szabályok törlését, majd csak az OWA (Outlook Web App) alkalmazásban hozzon létre és szerkesztsen szabályokat, amíg a probléma meg nem oldódik.

Ha nem tudja manuálisan törölni a szabályokat, az Outlook program indításakor az Outlook/cleanrules paranccsal is futtathatja az Outlook parancsát. Ezzel az ügyfél- és a kiszolgálói szabályt is törli. Törli az Outlook-profil összes fiókjának összes szabályát. Ezt a parancsot a Parancssori kapcsolók cikk tovább dokumentálja.

