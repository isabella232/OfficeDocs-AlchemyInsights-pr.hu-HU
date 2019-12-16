---
title: SharePoint Designer-csatlakozási problémák
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
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051715"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-csatlakozási problémák 

Ha a SharePoint Designer kapcsolódási problémákat tapasztal a SharePoint-webhelyeken, próbálja meg a következő közös megoldásokat.

1. lépés: Ellenőrizze, hogy a SharePoint Designer 2013 a [SharePoint Designer Service Pack 1 csomaggal](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) frissítve van-e és az [augusztusi 2, 2016 a SharePoint Designer 2013 frissítés](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2. lépés: a helyi gyorsítótárfájlok törlése:

1. Zárja be a SharePoint Designer 2013.

2. A helyi számítógépen távolítsa el a következő mappákban található fájlokat.

    - %APPDATA%\Microsoft\Web szolgál Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Nyit SharePoint Tervező 2013 és belép a számla újra-hoz lát ha ez szerkezet.

Lép 3: [képessé tesz korszerű hitelesítés részére hivatal 2013-ra Windows berendezés](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

4. lépés: a rendszergazdáknak engedélyezni kell az **egyéni parancsfájl** beállítást a SharePoint Admin Center beállításaiban a SharePoint Designer-kapcsolat engedélyezéséhez. További információt az [egyéni parancsfájl engedélyezése vagy tiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) című témakörben talál.


