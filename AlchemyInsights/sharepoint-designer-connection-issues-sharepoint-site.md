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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716894"
---
# <a name="sharepoint-designer-connection-issues"></a>A SharePoint Designer kapcsolódási problémák 

<p>Ha SharePoint Designer SharePoint-webhelyekhez csatlakozási problémákat tapasztalja, kérjük próbálja meg a következő közös megoldásokat.</p> <p><strong>1. lépés:</strong> <strong>Frissül, ellenőrizze a SharePoint Designer&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">A SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">A SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Frissítés a SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>2. lépés:</strong> <strong>A helyi gyorsítótárban található fájlok törlése</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Zárja be a SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">A helyi számítógépen keresse meg a következő mappákban tárolt fájlok eltávolítása.&nbsp;</li> <li style="font-weight: 400;">Kattintson a <strong>Start -&gt; futtassa a</strong> és az egyes található összes fájl törlése a helyek alatt.&nbsp;<br /><br />%APPDATA%\Microsoft\Web server Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Nyissa meg a SharePoint Designer 2013, és adja meg a fiók ismételten kattintva ellenőrizze, hogy az működik.</li> </ol> <p><strong>3. lépés:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>A Modern Office 2013 eszköz a Windows-hitelesítés engedélyezése</strong></a>&nbsp;</p> <p><strong>4. lépés:</strong> A <strong>rendszergazdák egyéni parancsfájl engedélyezi a SharePoint Designer kapcsolat engedélyezésére kell</strong>.</p> <p>Talál részletes leírást, példák és megfontolások <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">engedélyezése vagy tiltása egyéni parancsfájl</a>.&nbsp;</p>


