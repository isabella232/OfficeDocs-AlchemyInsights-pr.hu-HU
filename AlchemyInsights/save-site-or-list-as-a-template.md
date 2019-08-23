---
title: Webhely vagy lista mentése sablonként
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: a74d14f1743b9a016346f7bf0943523b1ab21f91
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551633"
---
# <a name="save-site-or-list-as-a-template"></a>Webhely vagy lista mentése sablonként

SharePoint-webhely sablonok olyan előre elkészített meghatározások körül üzleti célok figyelembe vételével tervezték. További információért lásd [a sablonok létrehozása a SharePoint-webhelyek különböző típusú](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Az alábbiakban néhány közös problémák/mentése egy webhely vagy lista vonatkozó sablonként a SharePoint Online.

**Mentés webhelyen vagy a listában sablon gomb nem elérhető vagy hiányzik**. 

- A rendszergazdák egyéni parancsfájl lehetővé kell sablon szolgáltatásainak használatához. Talál részletes leírást, példák és megfontolások [engedélyezése vagy tiltása egyéni parancsfájl](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- A mentési hely sablon parancs nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúra webhelyeket.


**A webhelysablon nem hozható létre vagy nem működik megfelelően**

- A sablon [funkció](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) hiányzik, és nem aktiválható. Ha a szolgáltatás nem érhető el az aktuális webhelycsoportban aktiválása, a webhelysablon webhelyet hozhat létre, nem használható.


- Ellenőrizze, hogy ha a listák vagy tárak nagyobb a [Listanézet küszöbén korlát](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 cikkek, webhelysablon létrehozásának blokkolni tudja.


- Előfordulhat, hogy a webhely használja túl sok erőforrást, és ezért a webhelysablon meghaladja az 50 megabájt (MB).


- Keresőoszlop használó listát származó adatokat megjelenítő problémák léptek fel. További tudnivalókért tanulmányozza a [sablon által létrehozott listán nem jeleníti meg a megfelelő keresési lista a SharePoint Online adatait](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).


További részletes információt a közös problémák és megoldások hivatkozás [létrehozása és használata a webhelysablonok](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)olvassa.

