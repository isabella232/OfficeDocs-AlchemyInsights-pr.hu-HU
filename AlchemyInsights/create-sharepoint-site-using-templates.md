---
title: Webhely létrehozása a SharePoint Online szolgáltatásban
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755310"
---
# <a name="create-sharepoint-sites-using-templates"></a>SharePoint-webhelyek létrehozása sablonokkal

A SharePoint webhelysablonok előre elkészített definíciók, amelyeket egy adott üzleti szükséglet köré terveztek. További információ: [sablonok használata különféle SharePoint-webhelyek létrehozásához](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Íme néhány gyakori probléma/megoldás a webhelyek vagy listák mentése sablonként a SharePoint Online szolgáltatásban. 

**A webhely/listasablon mentése gomb nem érhető el vagy hiányzik**

A rendszergazdáknak az egyéni parancsfájl engedélyezése lehetőséget kell engedélyezni a sablonszolgáltatások engedélyezéséhez. A részletes lépésekről, a példákat és megfontolásokat lásd: 

- [Egyéni parancsfájl engedélyezése vagy tiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- A webhely mentése sablonként parancs használata nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúrát használó webhelyeken.

**A webhelysablon nem hozható létre vagy nem működik megfelelően**

Lehet, hogy hiányzik egy [szolgáltatás](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , és a sablon nem aktiválható. Ha a szolgáltatás nem aktiválható az aktuális webhelycsoportban, a webhelysablonnal nem lehet webhelyet létrehozni.

- Ellenőriz-hoz lát ha akármi tetszik vagy könyvtárak kimagaslik a [oldalra dől kilátás korlátoz küszöb](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) -ból 5000 cikk mint ez tud fatuskó teremtés-ból egy telek mintadeszka.

- Előfordulhat, hogy a webhely túl sok erőforrást használ, ezért a webhelysablon túllépi a 50 MB-os korlátot.


- Problémák merülnek fel a keresőoszlopot használó listák adatainak megjelenítésekor. További információ: [a sablon által generált lista nem jeleníti meg a SharePoint Online megfelelő keresőlistájából származó adatokat](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

A gyakori problémákról és megoldásokról a [webhelysablonok létrehozása és használata című oldalon](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)olvashat részletesebben.



