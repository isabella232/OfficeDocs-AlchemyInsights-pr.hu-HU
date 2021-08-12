---
title: Ez a webhely nem érhető el – hibaüzenet jelenik meg, amikor megpróbál hozzáférni SharePoint webhelyhez böngészőből vagy Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 5f8861e85df21082329273237679e26a1b31ce694e11ad6407d4690d7caf2fc9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946653"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a>"Ez a webhely nem érhető el" hibaüzenet jelenik meg, amikor böngészőből vagy SharePoint próbál elérni Teams

A felhasználók "A webhely nem érhető el" hibaüzenet jelenhet meg, amikor böngészőből vagy webhelyről próbálnak SharePoint webhelyet elérni Teams. 

A probléma megoldása: 

1. Ellenőrizze, hogy a kezdőlap a Lomtárban vagy a másodszakaszban lévő lomtárban van-e, és állítsa vissza a lapot.

**Példa a lomtár közvetlen URL-címére:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx

1. Ha a kezdőlapot véglegesen eltávolítja a lomtárból, hozzon létre egy új webhelyet a Webhelylapok tárból, és tegye kezdőlapként. 

**Közvetlen URL-minta:**https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx