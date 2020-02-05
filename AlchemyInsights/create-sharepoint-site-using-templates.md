---
title: Webhely létrehozása a SharePoint Online-ban
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770425"
---
# <a name="create-sharepoint-sites-using-templates"></a>SharePoint-webhelyek létrehozása sablonok használatával

A modern kommunikációs vagy csoportwebhelyek nem támogatják a webhely sablonként való mentését. A sablonok használatáról további információt [a SharePoint-webhely mentése, letöltése és feltöltése sablonként](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)című témakörben talál.

Íme néhány gyakori probléma/megoldás a Webhely vagy lista sharepoint online sablonként való mentésével kapcsolatban. 

**Webhely/listasablon mentése gomb nem érhető el vagy hiányzik**

A rendszergazdáknak engedélyeznie kell az egyéni parancsfájlt a sablon szolgáltatásainak engedélyezéséhez. A részletes lépésekről, példákról és szempontokról lásd: 

- [Egyéni parancsfájl engedélyezése vagy lemegakadályozása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- A Webhely mentése sablonként parancs nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúráját használó webhelyeken.

**A webhelysablon nem hozható létre, vagy nem működik megfelelően**

Lehet, hogy a sablonból hiányzik egy [szolgáltatás,](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) és nem aktiválódik. Ha a funkció nem aktiválható az aktuális webhelycsoportban, a webhelysablon nem használható webhely létrehozására.

- Ellenőrizze, hogy a listák vagy tárak túllépik-e az 5000-es [listakorlát-korlátot,](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) mivel ez letilthatja a webhelysablon létrehozását.

- Lehet, hogy a webhely túl sok erőforrást használ, ezért a webhelysablon meghaladja az 50 MB-os korlátot.


- Probléma merül fel a keresoszlopot használó listából származó adatok megjelenítése korával kapcsolatban. További információt a Sablon által létrehozott lista nem [jelenít meg a SharePoint Online megfelelő keresőlistájának adatait.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

A gyakori problémákról és megoldásokról további információt a Webhelysablonok létrehozása és használata című, a [webhelysablonok létrehozása című,](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)a



