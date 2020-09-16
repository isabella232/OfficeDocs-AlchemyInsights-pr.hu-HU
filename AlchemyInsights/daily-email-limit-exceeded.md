---
title: A napi e-mail-korlát túllépve. A munkafolyamat fel van függesztve.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731565"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>A napi e-mail-korlát túllépve. A munkafolyamat fel van függesztve.

A hiba az alábbi esetekben fogadható el:

- Munkafolyamata van a SharePoint Online-ban, amely a SharePoint 2010 vagy a SharePoint 2013 munkafolyamat platform típusát használja.
- A munkafolyamat úgy van konfigurálva, hogy az egyéni e-mail-üzeneteket több mint 200-felhasználónál, naponta több mint 10 000 címzett, vagy percenként több mint 30 üzenetet küldjön.
- A munkafolyamat futtatásakor az e-maileket nem küldi el a program, és a következő viselkedést tapasztalja:
    - Ha a munkafolyamathoz a SharePoint 2013 platformját használja, tallózással keresse meg a **munkafolyamat állapota** lapot. A Munkafolyamat állapota lapon a **belső állapot** az **Indítás**értékre van állítva, az információs buborék pedig **nem tud elküldeni a címzetteknek**.

A probléma megoldásához állítsa be úgy a munkafolyamatot, hogy e-mail-üzeneteket küldjön az [Exchange Online-beli feladó korlátozásainak](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)túllépése nélkül. Használhatja például a munkafolyamatban a szünetet, elküldheti az e-mailt egy Microsoft 365-csoportba, egy terjesztési csoportba vagy egy levelezési biztonsági csoportba, vagy elküldheti az üzenetet legalább 200 címzettnek.


További információt a következő [cikkben](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)talál.

## <a name="related-topics"></a>Kapcsolódó témakörök
- [Folyamatábra létrehozása](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint és flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 