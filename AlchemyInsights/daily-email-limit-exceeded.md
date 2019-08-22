---
title: Napi e-mail határ túllépése. A munkafolyamat fel van függesztve.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514457"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Napi e-mail túllépi a megengedettet. A munkafolyamat fel van függesztve.

Ez a hiba megérkezhetnek az alábbi esetekben:

- A munkafolyamat a SharePoint Online használja a SharePoint 2010 vagy a SharePoint 2013 munkafolyamat platformtípusa van.
- A munkafolyamat egyéni e-mail üzenetet küldhet a felhasználók több mint 200 egyszerre, naponta 10 000-nél több címzettnek vagy egy perc alatt több mint 30 üzenetnél van beállítva.
- Amikor futtatja a munkafolyamatot, az e-mailt nem küldi el, és azt tapasztalja, hogy a következőképp működik:
    - A munkafolyamat segítségével a SharePoint 2013 platform típusa akkor keresse meg a **Munkafolyamat állapota** lapon. A munkafolyamat állapota oldalon **Belső állapota** **Elindítva**értékre van állítva, és az információs buborékban **nem sikerült elküldeni a címzetthez**.

A probléma kerülő megoldásához állítsa be a munkafolyamat e-mailek küldése a [küldő Exchange Online korlátok](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)túllépése nélkül. Például használja a munkafolyamat szünetet, az e-mailt küld egy Office 365, a terjesztési csoport vagy engedélyezett levelezési biztonsági csoport, vagy küldje el az üzenetet a címzetteknek kevesebb, mint 200 egyszerre.


További információt a következő [cikkben](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)talál.

## <a name="related-topics"></a>Kapcsolódó témakörök
- [Folyamat létrehozása](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [A SharePoint és az áram](https://flow.microsoft.com/blog/sharepoint-and-flow/) 