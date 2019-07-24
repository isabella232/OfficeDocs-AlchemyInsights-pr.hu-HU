---
title: A SharePoint Designer kapcsolódási problémák
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840553"
---
# <a name="sharepoint-designer-connection-issues"></a>A SharePoint Designer kapcsolódási problémák 

Ha a SharePoint Designer SharePoint-webhelyekhez csatlakozási problémákat tapasztalja, próbálkozzon a következő közös megoldásokat.

1. lépés: Ellenőrizze, hogy a SharePoint Designer 2013 frissül [a SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) és a [2016. augusztus 2. frissítés a SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2. lépés: A helyi gyorsítótárban található fájlok törlése:

1. Zárja be a SharePoint Designer 2013.

2. A helyi számítógépen a következő mappákban található összes fájl eltávolításához.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Nyissa meg a SharePoint Designer 2013, és adja meg a fiók ismételten kattintva ellenőrizze, hogy az működik.

3. lépés: a [Modern Office 2013 eszköz a Windows-hitelesítés engedélyezése](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

4. lépés: Rendszergazdák kell **Egyéni parancsfájl engedélyezi** a SharePoint felügyeleti központ beállításaiban a SharePoint Designer kapcsolat engedélyezésére. Lásd a [engedélyezése vagy tiltása egyéni parancsfájl](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) további információt.


