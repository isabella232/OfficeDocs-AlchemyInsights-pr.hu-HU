---
title: A munkafolyamat e-mailben nem küldi el
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
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059606"
---
# <a name="workflow-email-is-not-being-sent"></a>A munkafolyamat e-mailben nem küldi el

1. Munkafolyamatok e-mail az összes felhasználóra vagy csak bizonyos felhasználók nem kapnak, vagy megtekintheti a hiba **az e-mail üzenet nem küldhető el. Győződjön meg arról, hogy az e-mail rendelkezik-e érvényes címzettel**.

Ellenőrizze, hogy a felhasználó a **Mindenki** engedélyei csoport (felhasználói adatok listája) a webhelycsoport létezik.  Minta közvetlen URL-cím: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

- Ha a felhasználó nem létezik, ellenőrizze, hogy a felhasználó a lapba van aláírva. 
- Ha egy külső felhasználó, győződjön meg arról, hogy a meghívást elfogadták.
- Ha a felhasználó az engedélyek csoport létezik, ellenőrizze, hogy helyesek-e az e-mail címet.
- Ha a felhasználó e-mail címe nincs megadva itt, hozzon létre egy mintát értesítés az adott felhasználó, amely arra kényszeríti a felhasználói fiók a szinkronizálás a SharePoint felhasználói profilok a webhelycsoportban.
 
2. A munkafolyamatok e-mail küld a helycsoport-rendszergazdák azonban nem mások, és hibaüzenet jelenik **HTTP tilos <spam> <spam> ** <spam> <spam>.
 

Lásd: [Hozzáférés megtagadva az elküldött e-mail groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

Azt is ellenőrizze, hogy a **korlátozott hozzáférésű felhasználói engedély zárolási mód** webhelycsoport-szolgáltatás nincs bekapcsolva.

## <a name="related-topics"></a>Kapcsolódó témakörök
- [Folyamat létrehozása](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [A SharePoint és az áram](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


