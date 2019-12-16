---
title: A munkafolyamat-e-mail nem kerül elküldésre
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049375"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>A munkafolyamat-e-mail nem lett elküldve SharePoint-listához vagy-tárhoz

1. A munkafolyamatokból származó e-maileket nem küldi el a rendszer az összes felhasználónak vagy csak bizonyos felhasználóknak, vagy az **e-mail üzenetet nem lehet elküldeni. Győződj meg a elektronikus levél birtokol egy érvényes fogékony**.

    Ellenőrizze, hogy a felhasználó szerepel-e az adott webhelycsoport **minden személy** engedélyei csoportjában (felhasználói adatok listájában).  Minta közvetlen URL: https://<tenant>. sharepoint.com/sites/<sitename>/_layouts/15/People.aspx? MembershipGroupId = 0

    - Ha a felhasználó nem létezik, győződjön meg arról, hogy a felhasználó be van jelentkezve az oldalra. 
    - Ha külső felhasználó, akkor győződjön meg arról, hogy meghívásukat elfogadták.
    - Ha a felhasználó az engedélycsoportban is szerepel, ellenőrizze, hogy az e-mail cím helyes-e.
    - Ha a felhasználók e-mail címe nincs beállítva, akkor hozzon létre egy mintafigyelmeztetést arra a felhasználóra vonatkozóan, amely az adott felhasználói fióknak a SharePoint felhasználói profiljaihoz való szinkronizálását kényszeríti erre a webhelygyűjteményre.
 
2. A munkafolyamatokból érkező e-maileket a rendszer a webhelycsoport rendszergazdáinak küldi, de a többi felhasználónak nem, és a **http tiltott és <span>https:</span>//URL/_vti_bin/Client.xvc.Sp.Utilities.Utility.sendEmail**hibát látja.
 

    [Ha egy SharePoint-csoportnak küld e-mailt, tekintse át a hozzáférés megtagadva](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)választógombot.

    Ellenőrizze azt is, hogy a **korlátozott hozzáférésű felhasználói engedély zárolási módja** helycsoport-szolgáltatás nem aktív-e.


## <a name="related-topics"></a>Kapcsolódó témakörök
Szeretné kipróbálni a Microsoft flow-t a SharePoint Online szolgáltatásban?
- [Átfolyás létrehozása](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint-és adatfolyam](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


