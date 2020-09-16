---
title: A munkafolyamat-e-mailek küldése nem történik meg
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748991"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>SharePoint-lista vagy-tár esetén a program nem küldi el a munkafolyamat-e-maileket

1. A munkafolyamatokból származó e-maileket a program nem küldi el az összes felhasználónak vagy csak bizonyos felhasználóknak, vagy ha a hibaüzenet az, hogy az e-mail **nem küldhető el. Győződjön meg arról, hogy az e-mailhez érvényes címzett tartozik**

    Ellenőrizze, hogy a felhasználó megtalálható-e a webhelycsoporthoz tartozó **minden személy** engedélyei csoportban (felhasználói adatok listája).  Minta közvetlen URL: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Ha a felhasználó nem létezik, győződjön meg arról, hogy a felhasználó be van jelentkezve a lapra. 
    - Külső felhasználó esetén győződjön meg arról, hogy a meghívót elfogadták.
    - Ha a felhasználó létezik az engedélyek csoportban, ellenőrizze, hogy helyes-e az e-mail cím.
    - Ha a felhasználók e-mail-címe nincs beállítva, akkor hozzon létre egy, az adott felhasználóra vonatkozó figyelmeztetést, amely az adott felhasználói fiók szinkronizálását a SharePoint felhasználói profiljaiból ebbe a webhelycsoporthoz irányítja.
 
2. A munkafolyamatokból származó e-maileket a program a webhelycsoport rendszergazdáinak küldi el, a többi felhasználó számára azonban nem, és nem olvassa fel a ** <span>https:</span>//URL/_vti_bin/Client.xvc.Sp.Utilities.Utility.sendEmail**.
 

    Lásd: [hozzáférés megtagadva, amikor e-mailt küld egy SharePoint-csoportnak](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Ellenőrizze azt is, hogy a **korlátozott hozzáférésű felhasználói engedély zárolási módja** webhelycsoport-szolgáltatás nem aktív.


## <a name="related-topics"></a>Kapcsolódó témakörök
Szeretné kipróbálni a Microsoft flow-t a SharePoint Online-ban?
- [Folyamatábra létrehozása](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint és flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


