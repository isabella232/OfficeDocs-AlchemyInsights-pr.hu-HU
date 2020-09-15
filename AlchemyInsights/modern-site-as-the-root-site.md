---
title: Modern webhely root-webhelyként
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666872"
---
# <a name="modern-site-as-root-site"></a>Modern webhely root-webhelyként

Kezdtük egy új funkció kiépítését, amely lehetővé teszi, hogy a [klasszikus webhely gyökerét egy modern](https://docs.microsoft.com/sharepoint/modern-root-site)webhelyre cserélje. A [SPOSiteSwap hivatkozhat](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) arra, hogy a webhely helyét egy másik webhelyre cseréli az eredeti webhely archiválása közben. Mindkét csoportwebhely számára elérhető (nem kapcsolódhat egy csoporthoz) és egy kommunikációs webhelyhez.

>[!Important]
> A modern kommunikációs webhelyek létrehozásához ne törölje a klasszikus root-webhelyét. Ezt a Microsoft nem támogatja. A legfelső szintű webhely törlésekor a szervezet összes SharePoint-webhelye nem érhető el az összes felhasználó számára, amíg vissza nem állítja a webhelyet, illetve nem hozhat létre új webhelyet ugyanazon az URL-címen. Ezt a funkciót az üzenetközpont segítségével fogjuk kommunikálni. Várnia kell, hogy a funkció hamarosan be legyen kapcsolva a bérlői webhelyére.

## <a name="known-issues-with-swapping-sites"></a>A webhelyek cseréjével kapcsolatos ismert problémák
- Előfordulhat, hogy a cél egy rövid időre "not found" (HTTP 404) hibát ad vissza.
- A keresési index frissítéséhez a tartalmat újra kell bejárni. Ebben az esetben nincs szükség kézi lépésre, ezt automatikusan elvégezheti.
- A "statikus" hivatkozásokkal (például a fájlok szinkronizálására és a OneNote-fájlokra) függő bármit manuálisan kell kijavítani.
- Előfordulhat, hogy a Project Server-webhelyek érvényesítése szükséges ahhoz, hogy a rendszer továbbra is megfelelően társítsa őket. 
