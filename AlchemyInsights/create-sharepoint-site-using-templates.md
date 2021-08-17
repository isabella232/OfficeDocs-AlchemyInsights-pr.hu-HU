---
title: Webhely létrehozása az SharePoint-ban
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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057968"
---
# <a name="create-sharepoint-sites-using-templates"></a>Webhely SharePoint sablonok használatával

A modern kommunikációs és csoportwebhelyek nem támogatják a webhelyek sablonként való mentését. A sablonok használatáról a [SharePoint-webhely mentése, letöltése és feltöltése sablonként](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template) című témakörben olvashat bővebben.

A webhelyek vagy a lista sablonként való mentése a SharePoint Online-ban az alábbi gyakori problémákat/megoldásokat sorolja fel. 

**A Webhely mentése/listasablon gomb nem érhető el vagy hiányzik**

A rendszergazdáknak engedélyezniük kell az egyéni szkripteket a sablon szolgáltatásainak engedélyezéséhez. A részletes lépéseket, példákat és szempontokat lásd: 

- [Egyéni parancsprogram engedélyezése vagy letiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- A webhely mentése sablonként parancs nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúráját használó webhelyeken.

**A webhelysablon nem hozható létre vagy nem működik megfelelően**

Előfordulhat, hogy a sablonból hiányzik [egy funkció,](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) és nem aktiválódik. Ha a szolgáltatás nem aktiválható az aktuális webhelycsoportban, nem hozhat létre webhelyet a webhelysablonnal.

- Ellenőrizze, hogy nem haladja-e meg valamelyik lista vagy tár a [listanézet 5000 elemes küszöbértékét,](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) mivel az megakadályozhatja a webhelysablon létrehozását.

- Előfordulhat, hogy a webhely túl sok erőforrást használ, és a webhelysablon túllépi az 50 MB-os korlátot.


- Probléma lépett fel a keresési oszlopot használó lista adatainak a megjelenítésekor. A megoldásról [A sablon által létrehozott lista nem a megfelelő keresési listából jeleníti meg az adatokat a SharePoint Online-ban](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data) című témakörben olvashat.

A gyakori problémákról és megoldásokról további információt a Webhelysablonok létrehozása és [használata leírásában talál.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



