---
title: Webhely létrehozása a SharePoint Online-ban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732228"
---
# <a name="create-sharepoint-sites-using-templates"></a>SharePoint-webhelyek létrehozása sablonok használatával

A webhelyek sablonként való mentésének lehetőségét a modern kommunikációs vagy csoportwebhely-webhelyek nem támogatják. A sablonok használatáról további információt a [SharePoint-webhely mentése, letöltése és feltöltése sablonként](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)című témakörben talál.

Az alábbiakban néhány gyakori problémát és megoldást találhat a webhelyek vagy listák sablonként való mentésekor a SharePoint Online-ban. 

**A webhely/lista sablonjának mentése gomb nem érhető el vagy hiányzik**

A rendszergazdáknak engedélyezniük kell az egyéni parancsfájlok számára a sablonok funkcióinak használatát. A lépések részletes ismertetése: 

- [Egyéni parancsfájlok engedélyezése vagy letiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- A webhely mentése sablonként parancs nem érhető el, és problémákat okozhat a SharePoint Server közzétételi infrastruktúráját használó webhelyeken.

**A webhelysablon nem hozható létre vagy nem működik megfelelően**

Előfordulhat, hogy a sablon hiányzik egy [funkcióból](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , és nem aktiválódik. Ha a funkció nem érhető el az aktuális webhelycsoportban, a webhelysablonok nem használhatók webhelyek létrehozására.

- Ellenőrizze, hogy a lista vagy a tárak túllépik-e az 5000-elemek [listanézet-küszöbértékét](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , mivel ez letilthatja a webhelysablon létrehozását.

- Előfordulhat, hogy a webhely túl sok erőforrást használ, ezért a webhelysablon túllépi a 50 MB-os korlátot.


- Problémák vannak az olyan listákban, amelyek keresési oszlopot használnak. További információ: [a sablonok által generált lista nem jeleníti meg az adatokat a SharePoint Online-ban a megfelelő keresési listából](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

A gyakori problémákról és megoldásokról további információt a [webhelysablonok létrehozása és használata](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)című témakörben találhat.



