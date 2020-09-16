---
title: Webhely vagy lista mentése sablonként
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727533"
---
# <a name="save-site-or-list-as-a-template"></a>Webhely vagy lista mentése sablonként

A SharePoint-webhelysablonok előre elkészített definíciók, amelyek egy adott üzleti szükséglet köré lettek tervezve. További információt a [sablonok használata a különböző típusú SharePoint-webhelyek létrehozásához](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)című témakörben talál.

Az alábbiakban néhány gyakori problémát és megoldást találhat a webhelyek vagy listák sablonként való mentésekor a SharePoint Online-ban.

**A webhely/lista sablonjának mentése gomb nem érhető el vagy hiányzik**. 

- A rendszergazdáknak engedélyezniük kell az egyéni parancsfájlok számára a sablonok funkcióinak használatát. A lépések részletes ismertetését az [egyéni parancsfájlok engedélyezése vagy letiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)című témakörben találhatja meg.


- A webhely mentése sablonként parancs nem érhető el, és problémákat okozhat a SharePoint Server közzétételi infrastruktúráját használó webhelyeken.


**A webhelysablon nem hozható létre vagy nem működik megfelelően**

- Előfordulhat, hogy a sablon hiányzik egy [funkcióból](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , és nem aktiválódik. Ha a funkció nem érhető el az aktuális webhelycsoportban, a webhelysablonok nem használhatók webhelyek létrehozására.


- Ellenőrizze, hogy a lista vagy a tárak túllépik-e az 5000-elemek [listanézet-küszöbértékét](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , mivel ez letilthatja a webhelysablon létrehozását.


- Előfordulhat, hogy a webhely túl sok erőforrást használ, ezért a webhelysablon túllépi a 50 megabájtos (MB) korlátját.


- Problémák vannak az olyan listákban, amelyek keresési oszlopot használnak. További információ: [a sablonok által generált lista nem jeleníti meg az adatokat a SharePoint Online-ban a megfelelő keresési listából](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


A gyakori problémákról és megoldásokról további információt a [webhelysablonok létrehozása és használata](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)című témakörben találhat.

