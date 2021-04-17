---
title: A Microsoft Edge használata Chromium-böngészők alapján elektronikus adatfeladatokat exportálható
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
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834373"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>A Microsoft Edge használata Chromium-böngészők alapján elektronikus adatfeladatokat exportálható

Egy nemrégiben történt változás miatt a Microsoft Edge böngészőkben alapértelmezés szerint nem engedélyezett a ClickOnce támogatása. A Microsoft 365 Elektronikus adatok észlelése exportálási eszköz használatának folytatásához vagy a Microsoft Internet Explorert kell használnia, vagy engedélyeznie kell a ClickOnce-támogatást a Microsoft Edge-ben. 

A ClickOnce-támogatás engedélyezése a Microsoft Edge-ben Chromium alapján: 
1. A Microsoft Edge böngészőben látogasson el a edge://flags/#edge-click-once.
2. A ClickOnce támogatási csoportban módosítsa  az Alapértelmezett vagy a Letiltva értéket **Engedélyezve** **értékre.** 
3. A böngészőablak alján válassza az Újraindítás **lehetőséget.** <br>
 A módosítás a Microsoft Edge újraindítása után lép érvénybe. 

Erről és az exportálási eszköz telepítésének lépéséről a Tartalomkeresés [eredményének exportálásacímben található további információ.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)