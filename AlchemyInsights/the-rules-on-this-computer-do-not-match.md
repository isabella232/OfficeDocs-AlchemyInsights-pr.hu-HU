---
title: 'Hiba: A számítógépen nem egyeznek meg a szabályok'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782954"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Hiba: A számítógépen nem egyeznek meg a szabályok

Az ismert probléma frissített állapotának megtekintése: A számítógépen nem egyeznek meg a [Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) szabályai

Az Outlook csapata végrehajtott egy javítást a 12928.10000-es buildben. A javítás már az Insider Fast szinten van, és 2020. június végén a Havi csatornán is létezik. Miután a javított buildet javította, még egyszer megkérdezheti, hogy melyik szabályokat szeretné megtartani. Amikor a rendszer kéri, válassza a Kiszolgáló lehetőséget, majd menjen vissza az Outlookba, és engedélyezze újra a letiltott szabályokat.

A javítás elérhetővé válik, kérjük, használja az alábbi kerülő megoldást:

**Kerülő** megoldás: A legutóbbi jelentések szerint a probléma olyan ügyfeleknél fordult elő, akik csak az Outlook asztali verziójában hoztak létre ügyféloldali szabályokat. Ha a probléma továbbra is fennáll, érdemes törölni a szabályokat, majd csak az Outlook Web Appban létrehozni és szerkeszteni a szabályokat, amíg a probléma meg nem oldódik.

Ha nem tudja manuálisan törölni a szabályokat, futtathat egy Outlook-parancsot az Outlook elindítani a /cleanrules Outlook.exe futtatásával. Ezzel az ügyfél és a kiszolgáló szabályait is törli. Ezzel törli az Outlook-profilban az összes fiók összes szabályát. Ezt a parancsot a Parancssori kapcsolók cikkben is olvashatja.

