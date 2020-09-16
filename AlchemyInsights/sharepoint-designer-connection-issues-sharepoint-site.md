---
title: A SharePoint Designer kapcsolódási problémái
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727173"
---
# <a name="sharepoint-designer-connection-issues"></a>A SharePoint Designer kapcsolódási problémái 

Ha a SharePoint Designer a SharePoint-webhelyek kapcsolódási problémáit tapasztalja, próbálkozzon az alábbi általános megoldásokkal.

1. lépés: Ellenőrizze, hogy a SharePoint Designer 2013 frissült-e a [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) szervizcsomaggal és a sharepoint Designer [2013 augusztus 2-2016 frissítéssel](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Második lépés: a helyi gyorsítótár-fájlok törlése:

1. Zárja be a SharePoint Designer 2013.

2. A helyi számítógépen távolítsa el az összes olyan fájlt, amely az alábbi mappákban található.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Nyissa meg a SharePoint Designer 2013 alkalmazást, és adja meg ismét a fiókot, és ellenőrizze, hogy működik-e.

3. lépés: [a modern hitelesítés engedélyezése a Windows rendszerű eszközökön futó Office 2013](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)-ban.

4. lépés: a SharePoint Designer-kapcsolat engedélyezéséhez a rendszergazdáknak engedélyeznie kell az **egyéni parancsfájlokat** a SharePoint felügyeleti központ beállításaiban. További információt az [egyéni parancsfájlok engedélyezése vagy letiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) című témakörben talál.


