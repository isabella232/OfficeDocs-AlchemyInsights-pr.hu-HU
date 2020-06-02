---
title: A SharePoint Designer csatlakozási problémái
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511546"
---
# <a name="sharepoint-designer-connection-issues"></a>A SharePoint Designer csatlakozási problémái 

Ha a SharePoint Designer kapcsolattal kapcsolatos problémákat tapasztal a SharePoint-webhelyekkel, próbálkozzon az alábbi gyakori megoldásokkal.

1. lépés: Ellenőrizze, hogy a SharePoint Designer 2013 frissítve van-e a [SharePoint Designer Service Pack 1 szervizcsomaggal](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) és a [2016.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



2. lépés: A helyi gyorsítótárfájlok törlése:

1. Zárja be a SharePoint Designer 2013-at.

2. A helyi számítógépen távolítsa el az alábbi mappákban található összes fájlt.

    - %APPDATA%\Microsoft\Webkiszolgáló-bővítmények\Gyorsítótár
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Nyissa meg a SharePoint Designer 2013-at, és írja be újra a fiókot, és nézze meg, hogy működik-e.

3. lépés: [Modern hitelesítés engedélyezése az Office 2013-hoz Windows-eszközökön](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

4. lépés: A SharePoint Designer-kapcsolat engedélyezéséhez a Rendszergazdák nak engedélyeznie kell az **egyéni parancsfájlt** a SharePoint Felügyeleti központ beállításaiban. További információt az [Egyéni parancsfájl engedélyezése vagy lehetővé tévő engedélyezése](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) című témakörben talál.


