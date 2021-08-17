---
title: Nem küldi el a munkafolyamat e-mailjeit
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072522"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>A munkafolyamat e-mail-címe nem lesz elküldve egy SharePoint listához vagy tárhoz

1. A munkafolyamatok által küldött e-maileket nem küldi el az összes felhasználónak vagy csak adott felhasználóknak, vagy hibaüzenet jelenik meg: Az e-mail nem küldhető el. Győződjön meg arról, hogy **az e-mailnek van érvényes címzettje.**

    Ellenőrizze, hogy a felhasználó szerepel-e a **webhelycsoport** Minden ember engedélycsoportban (felhasználói adatok listájában).  Közvetlen URL-https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Ha a felhasználó nem létezik, győződjön meg arról, hogy a felhasználó be van jelentkezve a lapra. 
    - Külső felhasználó esetén győződjön meg arról, hogy elfogadta a meghívást.
    - Ha a felhasználó létezik az engedélycsoportban, ellenőrizze, hogy helyes-e az e-mail-cím.
    - Ha a felhasználók e-mail-címe nincs beállítva itt, akkor hozzon létre egy minta riasztást a felhasználóhoz, amely a felhasználói fiók szinkronizálását kényszeríti SharePoint felhasználói profilokból ebbe a webhelycsoportba.
 
2. A munkafolyamatok e-mailjei a webhelycsoportgazdáknak küldenek e-mailt, más felhasználóknak azonban nem, és a HTTP – Tiltott hibaüzenetet látják a **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail** címre.
 

    Lásd: Hozzáférés megtagadva, amikor e-mailt küld [egy SharePoint csoportnak.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Ellenőrizze azt is, hogy **a Korlátozott hozzáférésű** felhasználók engedélyeinek zárolási módja webhelycsoport-szolgáltatás nincs-e aktiválva.


## <a name="related-topics"></a>Kapcsolódó témakörök
Szeretné kipróbálni az Microsoft Flow az SharePoint-ban?
- [Új Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint és Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


