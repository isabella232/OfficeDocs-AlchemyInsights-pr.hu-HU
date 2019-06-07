---
title: A SharePoint Online jogosultsági szintek
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760695"
---
# <a name="sharepoint-designer-connection-issues"></a>A SharePoint Designer kapcsolódási problémák 

Ha SharePoint Designer SharePoint-webhelyekhez csatlakozási problémákat tapasztalja, kérjük próbálja meg a következő közös megoldásokat.

1. lépés: Ellenőrizze a SharePoint Designer frissül.

- [A SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [A SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Frissítés a SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

2. lépés: A helyi gyorsítótárban található fájlok törlése

- Zárja be a SharePoint Designer 2013.

- A helyi számítógépen keresse meg a következő mappákban tárolt fájlok eltávolítása.

- Kattintson a Start menü Futtatás és az egyes található összes fájl törlése az alábbi helyeken.

%APPDATA%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Nyissa meg a SharePoint Designer 2013, és adja meg a fiók ismételten kattintva ellenőrizze, hogy az működik.

3. lépés: [a Modern Office 2013 eszköz a Windows-hitelesítés engedélyezése](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

4. lépés: A rendszergazdák kell egyéni parancsfájl engedélyezi a SharePoint Designer kapcsolat engedélyezésére.

Talál részletes leírást, példák és megfontolások [engedélyezése vagy tiltása egyéni parancsfájl](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


