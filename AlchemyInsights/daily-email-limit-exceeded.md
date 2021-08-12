---
title: Túllépte a napi levelezési korlátot. A munkafolyamat fel van függesztve.
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
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914653"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Túllépte a napi levelezési korlátot. A munkafolyamat fel van függesztve.

Ez a hiba az alábbi esetekben jelenhet meg:

- A SharePoint Online-ban van egy olyan munkafolyamata, amely a SharePoint 2010 vagy SharePoint 2013-as munkafolyamat-platformtípust használja.
- A munkafolyamat úgy van konfigurálva, hogy egyszerre több mint 200 felhasználónak, naponta több mint 10 000 címzettnek vagy percenként több mint 30 üzenetnek küldjön egyéni e-mailt.
- A munkafolyamat futtatásakor az e-mail nem lesz elküldve, és a következő viselkedést veszi észre:
    - Az SharePoint 2013 platformtípust használó munkafolyamatok esetén a Munkafolyamat **állapota lapra kell** tallózni. A Munkafolyamat állapota lapon  a Belső állapot beállítás Elindítva **,** az információs buborék pedig a Nem lehet üzenetet küldeni **a címzettnek üzenet jelenik meg.**

A probléma megoldásához konfigurálja a munkafolyamatot úgy, hogy e-maileket küldjön anélkül, hogy túllépte volna a [Exchange Online korlátait.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Használhat például egy szüneteltetési funkciót a munkafolyamatban, elküldheti az e-mailt egy Microsoft 365-csoportnak, terjesztési csoportnak vagy levelezési címmel rendelkező biztonsági csoportnak, vagy egyszerre kevesebb mint 200 címzettnek küldheti el az üzenetet.


További információt a következő cikkben [talál.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Kapcsolódó témakörök
- [Új Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint és Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 