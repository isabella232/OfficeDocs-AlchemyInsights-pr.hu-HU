---
title: A munkafolyamat-e-mail küldése nem történik meg
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766135"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>A munkafolyamat-alapú e-mail nem küldő SharePoint-listához vagy tárhoz

1. A munkafolyamatokból származó e-mail eket a rendszer nem küldi el minden felhasználónak, vagy csak egy adott felhasználónak, vagy a hibaüzenet jelenik **meg: Az e-mail nem küldhető el. Győződjön meg arról, hogy az e-mailnek érvényes címzettje van.**

    Ellenőrizze, hogy a felhasználó létezik-e az adott webhelycsoport **Minden személyek** engedélycsoportjában (felhasználói adatok listájában).  Minta közvetlen<tenant>URL:https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? Tagsági csoportazonosító=0

    - Ha a felhasználó nem létezik, ellenőrizze, hogy a felhasználó be van-e jelentkezve a lapra. 
    - Ha külső felhasználóról van szó, győződjön meg arról, hogy a meghívást elfogadták.
    - Ha a felhasználó létezik az engedélycsoportban, ellenőrizze, hogy az e-mail cím helyes-e.
    - Ha a felhasználók e-mail címe nincs beállítva itt, akkor hozzon létre egy mintariasztást az adott felhasználó számára, amely kényszeríti az adott felhasználói fiók szinkronizálását a SharePoint felhasználói profiljaiból erre a webhelycsoportra.
 
2. A munkafolyamatokból származó e-maileket a rendszer elküldi a webhelycsoport rendszergazdáinak, de más felhasználóknak nem, és a HTTP Tiltott https hibát ** <span>látja:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Lásd: [Hozzáférés megtagadva, ha e-mailt küld egy SharePoint-csoportnak.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Ellenőrizze azt is, hogy a **korlátozott hozzáférésű felhasználói engedélyek zárolási módú** webhelycsoport szolgáltatása nem aktív-e.


## <a name="related-topics"></a>Kapcsolódó témakörök
Kiszeretné próbálni a Microsoft Flow-t a SharePoint Online-ban?
- [Folyamat létrehozása](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint és Folyamat](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


