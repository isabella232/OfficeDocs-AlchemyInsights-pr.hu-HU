---
title: Webhely vagy lista mentése sablonként
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752034"
---
# <a name="save-site-or-list-as-a-template"></a>Webhely vagy lista mentése sablonként

A SharePoint webhelysablonok előre elkészített definíciók, amelyeket egy adott üzleti szükséglet köré terveztek. További információ: [sablonok használata különféle SharePoint-webhelyek létrehozásához](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Íme néhány gyakori probléma/megoldás a webhelyek vagy listák mentése sablonként a SharePoint Online szolgáltatásban.

**A webhely/listasablon mentése gomb nem érhető el vagy hiányzik**. 

- A rendszergazdáknak az egyéni parancsfájl engedélyezése lehetőséget kell engedélyezni a sablonszolgáltatások engedélyezéséhez. A részletes lépésekről példákat és megfontolásokat az [egyéni parancsfájl engedélyezése vagy tiltása](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)című témakörben találhat.


- A webhely mentése sablonként parancs használata nem támogatott, és problémákat okozhat a SharePoint Server közzétételi infrastruktúrát használó webhelyeken.


**A webhelysablon nem hozható létre vagy nem működik megfelelően**

- Lehet, hogy hiányzik egy [szolgáltatás](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , és a sablon nem aktiválható. Ha a szolgáltatás nem aktiválható az aktuális webhelycsoportban, a webhelysablonnal nem lehet webhelyet létrehozni.


- Ellenőriz-hoz lát ha akármi tetszik vagy könyvtárak kimagaslik a [oldalra dől kilátás korlátoz küszöb](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) -ból 5000 cikk mint ez tud fatuskó teremtés-ból egy telek mintadeszka.


- Elképzelhető, hogy a webhely túl sok erőforrást használ, ezért a webhelysablon túllépi az 50 megabájt (MB) korlátot.


- Problémák merülnek fel a keresőoszlopot használó listák adatainak megjelenítésekor. További információ: [a sablon által generált lista nem jeleníti meg a SharePoint Online megfelelő keresőlistájából származó adatokat](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


További részletes információ a közös problémákról és megoldásokért kérjük, [hozzon létre és használjon webhelysablonokat](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

