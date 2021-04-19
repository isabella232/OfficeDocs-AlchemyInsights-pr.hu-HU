---
title: Segítségre van szüksége az e-mailek küldésének korlátozásával?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836281"
---
# <a name="need-help-with-email-sending-limits"></a>Segítségre van szüksége az e-mailek küldésének korlátozásával?

Az alábbiakban a szolgáltatásban kényszerített **tervezés szerinti küldési korlátokat** ismerheti meg. Ezekről a korlátozásokról további információt [itt talál](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).

- A kéretlen tömeges üzenetek kézbesítésének visszaszorítása érdekében felhasználónkénti **címzettarányos korlátokat alkalmazunk minden kimenő és belső üzenetre**. Ez a korlát az összes termékváltozatban **10 000 címzett naponta**.  Azok az ügyfelek, akiknek valódi tömeges kereskedelmi e-mailt (például hírleveleket az ügyfeleknek) kell küldeniük, az e szolgáltatásokra specializálódott külső szolgáltatókat kell igénybe venniük.
    - **Megjegyzés**: Miután elérte a címzettek arányának korlátját, a rendszer nem tud üzenetet küldeni a postaládából, amíg a korlát alá nem esik azoknak a címzetteknek a száma, akiknek az elmúlt 24 órában üzenetet küldött. A felhasználó csak ezt a pontot elérve tud majd üzeneteket küldeni.
- A rendszer a **percenkénti 30 üzenet** üzenetarány-korlátot alkalmazza az összes termékváltozat esetén. Ez meghatározza, hogy egy felhasználó hány üzenetet küldhet egy megadott időszakon belül az Exchange Online-fiókjából.
- A **Címzett, Másolatot kap és Titkos másolat mezőben engedélyezett címzettek maximális száma** az összes termékváltozatban egyetlen e-mail esetén **1000 címzett** lehet. A korlát testreszabásához [lépjen ide](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).
