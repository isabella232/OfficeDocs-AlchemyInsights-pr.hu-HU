---
title: Napi elektronikus levél korlátoz kimagaslik. A munkafolyamat felfüggesztve.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053119"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Napi email limit túllépve. A munkafolyamat felfüggesztve.

A hiba a következő helyzetekben jelenhet meg:

- Olyan munkafolyamatot használ a SharePoint Online szolgáltatásban, amely a SharePoint 2010 vagy SharePoint 2013 munkafolyamat-platformtípust használja.
- A munkafolyamat úgy van beállítva, hogy egy egyéni e-mail üzenetet több mint 200 felhasználók részére küld egy időben, több mint 10 000 címzettek naponta, vagy több mint 30 üzenet percenként.
- A munkafolyamat futtatásakor az e-mail üzenetet a rendszer nem küldi el, és a következő viselkedést észleli:
    - A SharePoint 2013 platformtípust használó munkafolyamat esetén tallózással keresse meg a **munkafolyamat állapota** lapot. A Munkafolyamat állapota lapon a **belső állapot** beállítása **elindítva**, az információs buborék pedig **nem tud elküldeni a címzettnek**.

A probléma kerülő megoldásához konfigurálja úgy a munkafolyamatot, hogy az e-mail üzeneteket az [Exchange Online küldőjéhez megadott korlátok](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)túllépése nélkül küldje el. Például szüneteltetheti a munkafolyamatot a munkafolyamatban, elküldheti az e-mailt egy Office 365-csoportnak, terjesztési csoportnak vagy levelezési csoport számára engedélyezett biztonsági csoportnak, illetve elküldheti az üzenetet egyszerre kevesebb, mint 200 címzettnek.


További információt a következő [cikkben](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)találhat:

## <a name="related-topics"></a>Kapcsolódó témakörök
- [Átfolyás létrehozása](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint-és adatfolyam](https://flow.microsoft.com/blog/sharepoint-and-flow/) 