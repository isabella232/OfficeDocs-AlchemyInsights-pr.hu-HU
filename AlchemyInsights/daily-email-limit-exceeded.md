---
title: A napi e-mail korlát túllépve. A munkafolyamat fel van függesztve.
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
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580335"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Napi e-mail korlát túllépve. A munkafolyamat fel van függesztve.

Ez a hiba a következő esetekben jelenhet meg:

- A SharePoint 2010 vagy a SharePoint 2013 munkafolyamat-platformtípusát használó SharePoint Online-munkafolyamattal rendelkezik.
- A munkafolyamat úgy van beállítva, hogy egyszerre több mint 200 felhasználónak, naponta több mint 10 000 címzettnek vagy percenként több mint 30 üzenetnek küldjön üzenetet.
- A munkafolyamat futtatásakor a rendszer nem küldi el az e-mailt, és a következő viselkedést veszi észre:
    - A SharePoint 2013 platformtípust használó munkafolyamatok esetén keresse meg a **Munkafolyamat állapota** lapot. A Munkafolyamat állapota lapon a **Belső állapot** beállítása **Elindítva**, és az információs buborék ban látható **A nem küldhető el a címzettnek**.

A probléma kerülő megoldásához konfigurálja úgy a munkafolyamatot, hogy az [Exchange Online feladói korlátainak](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)túllépése nélkül küldjön e-maileket. Például szüneteltetheti a munkafolyamatot, elküldheti az e-mailt egy Microsoft 365-csoportnak, egy terjesztési csoportnak vagy egy levelezést engedélyező biztonsági csoportnak, vagy egyszerre kevesebb mint 200 címzettnek.


További információt a következő [cikkben](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)talál.

## <a name="related-topics"></a>Kapcsolódó témakörök
- [Folyamat létrehozása](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint és Folyamat](https://flow.microsoft.com/blog/sharepoint-and-flow/) 