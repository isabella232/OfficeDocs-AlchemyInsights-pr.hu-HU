---
title: Hozzáférés korlátozása a SharePointban vagy a OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700457"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hozzáférés korlátozása a SharePointban vagy a OneDrive

A SharePoint Online-ban és az OneDrive-szolgáltatásokban többféleképpen korlátozhatja a hozzáférést. Ezek a különféle hozzáférési korlátozási módszerek alább láthatók. 

**Jogosultság korlátozás**

A SharePoint Online-ban és a OneDrive vállalati verzióban csak a webhelyek, a fájlok és a mappák hozzáférését korlátozzuk, ha hozzáférést szeretne adni azokhoz a csoportokhoz/egyénekhez, akiknek hozzáféréssel kell rendelkezniük.

- [SharePoint-lista vagy-tár engedélyeinek testreszabása](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [A SharePoint-webhely engedélyeinek testreszabása](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Almappa engedélyeinek módosítása](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Nem kezelt eszközök hozzáférésének kezelése](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint-vagy globális rendszergazdaként letilthatja vagy korlátozhatja a SharePoint-és OneDrive-tartalmakat nem felügyelt eszközökről

**Hálózati hely korlátozás**

IT-rendszergazdaként a SharePoint-és OneDrive-erőforrásokhoz való hozzáférést a megbízhatóként megadott hálózati helyek alapján szabályozhatja. Ez más néven hely-alapú házirend. További információért olvassa el [a SharePoint Online és a OneDrive-adatok elérésének szabályozása hálózati hely alapján](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) című témakört.

**Webhely zárolásának korlátozása** 

A SharePoint Online-ban lehetősége van egy webhelycsoport zárolására, így senki sem férhet hozzá. Ez a beállítás a PowerShellen keresztül és a [SharePoint Online felügyeleti rendszerhéjon](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) keresztül érhető el a [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate tulajdonság használatával.

**Webhelyek és alwebhelyek létrehozásának korlátozása a felhasználóknak**

SharePoint-rendszergazdaként vagy globális rendszergazdává teheti a felhasználókat, hogy saját SharePoint-webhelyeket hozzanak létre és felügyelnek, meghatározhatja, hogy milyen típusú webhelyeket hozhat létre, és adja meg a webhelyek helyét. További információért olvassa el a [webhely létrehozása a SharePoint Online-ban](https://docs.microsoft.com/sharepoint/manage-site-creation) című témakört.

