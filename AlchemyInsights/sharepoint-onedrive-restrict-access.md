---
title: Hozzáférés korlátozása a SharePointban vagy a OneDrive-on
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692767"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hozzáférés korlátozása a SharePointban vagy a OneDrive-on

A SharePoint Online-szolgáltatásokhoz/OneDrive-szolgáltatásokhoz való hozzáférés számos módon korlátozhatja a hozzáférést. Ezeket a különböző hozzáférés-korlátozási módszereket az alábbiakban ismertetjük. 

**Engedélykorlátozás**

A SharePoint Online-ban és a OneDrive Vállalati verzióban úgy korlátozzuk a hozzáférést az olyan elemekhez, mint a webhelyek, fájlok és mappák, ha csak azoknak a csoportoknak/személyeknek biztosítunk hozzáférést, akiknek hozzáféréssel kell rendelkezniük.

- [SharePoint-lista vagy tár engedélyeinek testreszabása](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint-webhely engedélyeinek testreszabása](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Almappa engedélyeinek módosítása](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Nem kezelt eszközök hozzáférésének kezelése](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint- vagy globális rendszergazdaként letilthatja vagy korlátozhatja a SharePoint- és OneDrive-tartalmakhoz való hozzáférést nem felügyelt eszközökről (amelyek nem hibrid AD-hez csatlakoztak vagy nem kompatibilisek az Intune-ban).

**Hálózati hely korlátozása**

Informatikai rendszergazdaként szabályozhatja a SharePoint- és OneDrive-erőforrásokhoz való hozzáférést a megvetett hálózati helyek alapján. Ezt helyalapú házirendnek is nevezik. További információt a [SharePoint Online-adatokhoz való hozzáférés szabályozása a hálózati hely alapján](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) című témakörben talál.

**Webhelyzárolás korlátozása** 

A SharePoint Online-on belül zárolhat egy webhelycsoportot, így senki sem férhet hozzá. Ez a PowerShell és a [SharePoint Online felügyeleti rendszerhéj](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) on keresztül a [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState tulajdonság használatával van beállítva.

**A felhasználók webhelyek vagy alwebhelyek létrehozásának korlátozása**

SharePoint-rendszergazdaként vagy globális rendszergazdaként lehetővé teheti a felhasználók számára, hogy saját SharePoint-webhelyeket hozzanak létre és felügyeljenek, meghatározzák, hogy milyen webhelyeket hozhatnak létre, és megadhatja a webhelyek helyét. További információt a [Webhelylétrehozásának kezelése a SharePoint Online-ban című témakörben talál.](https://docs.microsoft.com/sharepoint/manage-site-creation)

