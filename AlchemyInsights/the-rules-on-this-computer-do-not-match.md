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
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981115"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Hiba: A számítógépen nem egyeznek meg a szabályok

Az ismert probléma frissített állapotáról [](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) A számítógépen nem egyező szabályok a Microsoft-fiókban Exchange

A Outlook 12928.10000-es buildben végrehajtott egy javítást. A javítás már az Insider Fast szinten van, és 2020. június végén a Havi csatornán is létezik. Miután a javított buildet javította, még egyszer megkérdezheti, hogy melyik szabályokat szeretné megtartani. Amikor a rendszer kéri, válassza a Kiszolgáló lehetőséget, majd Outlook újra engedélyezni a letiltott szabályokat.

A javítás elérhetővé válik, kérjük, használja az alábbi kerülő megoldást:

**Kerülő** megoldás: A legutóbbi jelentések szerint a probléma olyan ügyfeleknél fordult elő, akik csak az asztali Outlook hoztak létre. Ha a probléma továbbra is fennáll, érdemes törölni a szabályokat, majd csak az Outlook Web Appban (Outlook Web App) létrehozni és szerkeszteni a szabályokat, amíg a probléma meg nem oldódik.

Ha nem tudja manuálisan törölni a szabályokat, futtathat egy Outlook parancsot a Outlook /cleanrules Outlook.exe futtatásával. Ezzel az ügyfél és a kiszolgáló szabályait is törli. Ezzel törli a profilban a fiók összes Outlook szabályt. Ezt a parancsot a Parancssori kapcsolók cikkben is olvashatja.

