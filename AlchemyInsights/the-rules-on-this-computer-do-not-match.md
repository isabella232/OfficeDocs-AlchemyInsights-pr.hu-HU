---
title: 'Hiba: a számítógépen lévő szabályok nem egyeznek meg'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690965"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Hiba: a számítógépen lévő szabályok nem egyeznek meg

Ha az ismert probléma frissített állapotát szeretné látni, tanulmányozza [a számítógépen lévő szabályok nem egyeznek meg a Microsoft Exchange szabályaival](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Az Outlook csapata végrehajtotta a 12928,10000-es verzió javítását. A javítás már az Insider Fast-on van, és a havi csatorna 2020 június végén fog kinézni. Miután megadta a fix összeállítást, a következő üzenet jelenik meg: "milyen szabályok szerint szeretné megőrizni az időt". Válassza a kiszolgáló lehetőséget, amikor a rendszer kéri, majd térjen vissza az Outlookba, és engedélyezze újra a letiltott szabályokat.

Amíg a javítás elérhetővé nem válik, kérjük, használja az alábbi kerülő megoldást:

**Kerülő megoldás**: a legutóbbi jelentésekben a probléma abban az esetben fordult elő, ha az asztali Outlookban csak az ügyfél-szabályokat hozta létre. Ha továbbra is fennáll a probléma, fontolja meg a szabályok törlését, majd csak az OWA (Outlook Web App) alkalmazásban hozzon létre és szerkesszen szabályokat a probléma megoldásához.

Ha nem tudja törölni a szabályokat manuálisan, akkor futtathatja az Outlook parancsát, ha a Outlook.exe/cleanrules. futtatja az Outlookot. Ez az ügyfél-és kiszolgálói szabályok törlését is törli. Törli az Outlook-profil összes fiókjának összes szabályát. Ezt a parancsot részletesebben a parancssori kapcsolók című cikk ismerteti.

