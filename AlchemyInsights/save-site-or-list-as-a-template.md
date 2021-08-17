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
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109206"
---
# <a name="save-site-or-list-as-a-template"></a>Webhely vagy lista mentése sablonként

SharePoint webhelysablonok adott üzleti hez tervezett, előre létrehozott definíciók. További információ: Sablonok használata különböző típusú webhely [SharePoint létrehozásához.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Íme néhány gyakori probléma/megoldás, amely a webhely vagy lista sablonként való mentésével kapcsolatban SharePoint online.

**A Webhely mentése/listasablon mentése gomb nem érhető el vagy nem található.** 

- A rendszergazdáknak engedélyezniük kell az egyéni szkripteket a sablon szolgáltatásainak engedélyezéséhez. A részletes lépéseket, példákat és szempontokat az Egyéni parancsfájlok engedélyezése [és engedik](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)meg.


- A webhely mentése sablonként parancs nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúráját használó webhelyeken.


**A webhelysablon nem hozható létre vagy nem működik megfelelően**

- Előfordulhat, hogy a sablonból hiányzik [egy funkció,](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) és nem aktiválódik. Ha a szolgáltatás nem aktiválható az aktuális webhelycsoportban, nem hozhat létre webhelyet a webhelysablonnal.


- Ellenőrizze, hogy nem haladja-e meg valamelyik lista vagy tár a [listanézet 5000 elemes küszöbértékét,](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) mivel az megakadályozhatja a webhelysablon létrehozását.


- Előfordulhat, hogy a webhely túl sok erőforrást használ, ezért a webhelysablon meghaladja az 50 megabájtos korlátot.


- Probléma lépett fel a keresési oszlopot használó lista adatainak a megjelenítésekor. További információ: A sablon által létrehozott lista nem a megfelelő keresési listából jeleníti meg az adatokat a [SharePoint online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


A gyakori problémákról és megoldásokról további információt a Webhelysablonok létrehozása és [használata leírásában talál.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

