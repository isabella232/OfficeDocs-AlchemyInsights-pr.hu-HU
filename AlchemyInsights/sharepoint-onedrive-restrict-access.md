---
title: Hozzáférés korlátozása a SharePoint-ban OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093832"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hozzáférés korlátozása a SharePoint-ban OneDrive

Sokféleképpen korlátozhatja a hozzáférést az SharePoint/OneDrive szolgáltatásokhoz. Ezeket a különböző hozzáférési korlátozási módszereket alább ismertetjük. 

**Engedélykorlátozás**

Az SharePoint Online-ban és a OneDrive Vállalati verzió-ban úgy korlátozzuk a hozzáférést az elemekhez, például a webhelyekhez, fájlokhoz és mappákhoz, hogy csak azoknak a csoportoknak/személyeknek biztosítunk hozzáférést, akiknek hozzáférést kell okkal látniuk.

- [Lista vagy tár engedélyeinek SharePoint testreszabása](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Webhely SharePoint testreszabása](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Almappa engedélyeinek módosítása](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Nem kezelt eszközök hozzáférésének kezelése](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

A SharePoint- vagy globális rendszergazdaként letilthatja vagy korlátozhatja a nem felügyelt eszközökről származó SharePoint- és OneDrive-tartalmakhoz való hozzáférést (azokét, amelyek nem csatlakoztak vagy kompatibilisek az Intune-ban a hibrid AD-hez).

**Hálózati hely korlátozása**

Rendszergazdaként szabályozhatja a megbízható SharePoint és OneDrive erőforrásokhoz való hozzáférést. Ezt helyalapú házirendnek is nevezik. További információ: Hozzáférés [szabályozása](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) az online SharePoint és OneDrive adatokhoz hálózati hely alapján

**Webhely zárolásának korlátozása** 

A SharePoint Online-on belül lehetősége van zárolni a webhelycsoportokat, így senki más nem férhet hozzá. Ezt a PowerShellen és a SharePoint Online felügyeleti [rendszerhéjon](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) keresztül lehet beállítani a [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState tulajdonság használatával.

**A felhasználók korlátozása webhelyek vagy alwebhelyek létrehozására**

Rendszergazdaként vagy globális rendszergazdaként SharePoint felhasználók létrehozhatják és felügyelheti saját SharePoint-webhelyeiket, meghatározhatja, hogy milyen típusú webhelyeket hozhatnak létre, és megadhatja a webhelyek helyét. További információt a Webhelykészítés kezelése a [SharePoint webhelyen SharePoint.](https://docs.microsoft.com/sharepoint/manage-site-creation)

