---
title: A SharePoint Online webhely létrehozása
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753710"
---
# <a name="create-sharepoint-sites-using-templates"></a>Sablonok használata SharePoint-webhelyek létrehozása

SharePoint-webhely sablonok olyan előre elkészített meghatározások körül üzleti célok figyelembe vételével tervezték. További információért lásd [a sablonok létrehozása a SharePoint-webhelyek különböző típusú](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Az alábbiakban néhány közös problémák/mentése egy webhely vagy lista vonatkozó sablonként a Sharepoint Online. 

**Webhelyen vagy a listában sablon gomb nem érhető el vagy nincs megadva**

A rendszergazdák egyéni parancsfájl lehetővé kell sablon szolgáltatásainak használatához. Részletes leírást, példák és szempontok: 

- [Engedélyezhetjük vagy letilthatjuk az egyéni parancsfájl](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- A mentési hely sablon parancs nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúra webhelyeket.

A webhelysablon nem hozható létre vagy nem működik megfelelően.

A sablon [funkció](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) hiányzik, és nem aktiválható. Ha a szolgáltatás nem érhető el az aktuális webhelycsoportban aktiválása, a webhelysablon webhelyet hozhat létre, nem használható.

- Ellenőrizze, hogy ha a listák vagy tárak nagyobb a [Listanézet küszöbén korlát](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 cikkek, webhelysablon létrehozásának blokkolni tudja.

- Előfordulhat, hogy a webhely használja túl sok erőforrást, és ezért a webhelysablon meghaladja az 50 MB-os korlátot.


- Keresőoszlop használó listát származó adatokat megjelenítő problémák léptek fel. További tudnivalókért tanulmányozza a [sablon által létrehozott listán nem jeleníti meg a megfelelő keresési lista a SharePoint Online adatait](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Részletes információt a közös problémák és megoldások ellenőrizze a [webhely sablonok létrehozása és használata](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



