---
title: SharePoint A Tervező csatlakozási problémái
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942027"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint A Tervező csatlakozási problémái 

Ha SharePoint Tervező csatlakozási problémákat tapasztal a SharePoint, próbálkozzon az alábbi gyakori megoldásokkal.

1. lépés: Ellenőrizze, hogy a SharePoint Designer 2013 frissül-e az [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) szervizcsomaggal és a SharePoint Designer [2013 2016. augusztus 2-i frissítéssel.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



2. lépés: A helyi gyorsítótárfájlok törlése:

1. Zárja be SharePoint Designer 2013-as tervezőt.

2. A helyi számítógépen távolítsa el az alábbi mappákban található összes fájlt.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Nyissa SharePoint Designer 2013-ban, és adja meg ismét a fiókot, és nézze meg, hogy működik-e.

3. lépés: [A modern hitelesítés engedélyezése Office 2013-ban Windows eszközökön.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

4. lépés: A  rendszergazdáknak engedélyeznie kell az egyéni parancsfájlokat a SharePoint Felügyeleti központ beállításai között ahhoz, hogy engedélyezné a SharePoint kapcsolatot. További információt az Egyéni parancsfájl engedélyezése vagy [írásának](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) engedik meg.


