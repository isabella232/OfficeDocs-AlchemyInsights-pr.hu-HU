---
title: Postaláda fogadásának korlátja kényszerítve
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/31/2021
ms.locfileid: "59315899"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Postaláda fogadásának korlátja kényszerítve

A Microsoft nemrégiben kényszeríteni kezdte a postaládánkénti 3600 üzenet/óra küszöbértékét. További információt a Korlátozások Exchange Online [tartalmaz.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 órán belül több mint 3600 üzenetet megkapó postaládákat a rendszer a következő 60 percre lekordul. 

Emellett a feladó és a címzettek által megadott párokra (SRP) vonatkozó korlát, amely letiltja az Microsoft 365 egy adott feladótól érkező Microsoft 365 üzeneteket. Ha egy feladó a teljes küszöbérték 33%-át vagy 1200 üzenetet küld görgetőóránként egy adott címzettnek, a termékkulccsal kapcsolatos korlát indul el, és a postaláda többé nem fogadja el az adott feladótól érkező üzeneteket. Fontos tudni, hogy:

- Ez a korlát a más bérlőktől, helyszíni vagy internetes feladóktól kapott e-mailekre vonatkozó alkalmazás.
- A postaládába küldött e-mailek kézbesítése 60 percre le van tiltva. 
- E postaládák feladói egy nem kézbesítésről szóló jelentést kapnak (5.2.121 vagy 5.2.122), amely arról számol be, hogy a postaláda túllépte a maximális kézbesítési küszöböt. A bérlői fiókon belüli (ugyanazon bérlőn belüli) levelek kézbesítése továbbra is meg fog folytatódni.
- A SRP korlát alkalmazásakor a fogadó postaláda továbbra is elfogadja a többi feladótól érkező üzeneteket.

A rendszergazdák figyelik az aktuális postaláda-tevékenységeket egy új jelentés és Exchange Felügyeleti központ "A fogadási korlátokat túllépő postaládák" című témakörben. A betekintés csak akkor jelenik meg, ha egy bérlőnek vannak postaládái, míg a jelentés mindig megjelenik az irányítópulton, de üres, hacsak nem a bérlőnek vannak postaládái.

A meglátási korlátokról további információt A fogadási korlátokat túllépő postaládák az [új Exchange 2016-ban (EAC)](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

A fogadási korlátok túllépése jelentésről további információt a Fogadási korlátokat túllépő postaládák jelentés az [új Exchange 2010-jelentésben](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)található.