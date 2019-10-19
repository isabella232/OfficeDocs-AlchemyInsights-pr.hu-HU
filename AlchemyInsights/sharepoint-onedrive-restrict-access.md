---
title: Hozzáférés korlátozása a SharePoint vagy az OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750666"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hozzáférés korlátozása a SharePoint vagy az OneDrive

A SharePoint Online/OneDrive szolgáltatásokhoz való hozzáférést sokféleképpen korlátozhatja. Ezek a különféle hozzáférés-korlátozási módszerek az alábbiakban kerülnek ismertetásra. 

**Engedélykorlátozás**

-Ban SharePoint Online és OneDrive részére teendő, mi korlátoz belépés-hoz cikk szeret telek, fájlokat és tartók mellett egyetlen biztosít belépés-hoz azok csoportok/egyének ki kellet volna volna belépés.

- [SharePoint-lista vagy-tár engedélyeinek testreszabása](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [A SharePoint-webhelyek engedélyeinek testreszabása](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Almappára vonatkozó engedélyek módosítása](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Nem kezelt eszközök hozzáférésének kezelése](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Mint egy SharePoint vagy világ-admin-ban Hivatal 365, tudod fatuskó vagy korlátoz belépés-hoz SharePoint és OneDrive elégedett-ból nem kezelt berendezés (azok nem hibrid hirdetés összekapcsolt vagy szolgálatkész-ban Intune).

**Hálózati helykorlátozás**

A SharePoint és OneDrive erőforrásokhoz való hozzáférést az informatikai rendszergazdaként a megbízható hálózati helyek alapján szabályozhatja. Helyalapú házirend néven is ismert. További információt a [SharePoint Online és az OneDrive adataihoz való hozzáférés szabályozása a hálózati hely alapján](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) című témakörben talál.

**Webhely-zárolási korlátozás** 

A SharePoint Online szolgáltatásban lehetősége van arra, hogy zárolja a webhelygyűjteményt, így nincs hozzáférése. Ez a PowerShell eszközzel és a [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) segítségével állítható be, a [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate tulajdonsággal.

**Webhelyek vagy alwebhelyek létrehozásának korlátozása a felhasználók számára**

A SharePoint admin vagy az Office 365 globális rendszergazda segítségével a felhasználók létrehozhatják és felügyelhetik saját SharePoint-webhelyeiket, meghatározhatják, hogy milyen webhelyeket hozhatnak létre, és meghatározhatják a webhelyek helyét. További információkért tekintse [meg a webhelyek létrehozásának kezelése a SharePoint Online szolgáltatásban](https://docs.microsoft.com/sharepoint/manage-site-creation) című témakört.

