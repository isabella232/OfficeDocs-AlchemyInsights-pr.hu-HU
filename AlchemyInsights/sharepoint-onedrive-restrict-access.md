---
title: Korlátozza a hozzáférést a SharePoint- vagy OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559879"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Korlátozza a hozzáférést a SharePoint- vagy OneDrive

Számos módon való hozzáférés korlátozása a SharePoint Online/OneDrive szolgáltatások. E különböző hozzáférési korlátozás módszerek az alábbiakban vázolt. 

**Engedélyek korlátozása**

A SharePoint Online és az üzleti OneDrive azt korlátozza a hozzáférést elemekhez, például a webhelyek, fájlok és mappák csak a csoportok/személyek rendelkezzenek hozzáféréssel való hozzáférés biztosítása által.

- [SharePoint-lista vagy tár engedélyeinek testreszabása](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [A SharePoint webhely engedélyeinek testreszabására](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Almappa engedélyeinek módosítása](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Nem kezelt eszközök hozzáférésének kezelése](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint vagy az Office 365 globális rendszergazda zárolhatja vagy korlátozza a hozzáférést a SharePoint-és OneDrive a nem kezelt eszközök (a hibrid illesztett vagy kompatibilis az Intune AD).

**Hálózati hely korlátozás**

INFORMATIKAI rendszergazdaként szabályozhatja a meghatározott hálózati helyeken megbízható alapuló SharePoint és OneDrive erőforrásokhoz való hozzáférést. Ez a hely alapú házirend néven is ismert. További információt talál [a SharePoint Online és a OneDrive adatok hálózati hely alapján való hozzáférés szabályozása](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Webhelykorlátozás zárolása** 

SharePoint Online belül, hogy a számítógép zárolásához a webhelycsoportot, így ne hozzáférése van. A PowerShell és a [SharePoint Online felügyeleti rendszerhéj](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) segítségével a [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState tulajdonság értéke.

**Webhelyek és alwebhelyek létrehozását követően a felhasználók korlátozása**

A SharePoint felügyeleti vagy Office 365 globális felügyeleti lehetővé teszik a felhasználók létrehozása és a saját SharePoint-webhelyek felügyelete, meghatározza, milyen típusú webhelyeket hozhatnak létre, és a webhelyek elérési útja. További információért lásd [kezelés webhely létrehozása a SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

