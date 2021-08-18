---
title: Modern webhely mint gyökérwebhely
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
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327604"
---
# <a name="modern-site-as-root-site"></a>Modern webhely gyökérwebhelyként

Megkezdtük egy új funkció bevezetését, amely lehetővé teszi, hogy felcserélje a klasszikus webhely gyökérwebhelyét [egy modern webhelyről.](https://docs.microsoft.com/sharepoint/modern-root-site) Az [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) használatával felcserélje egy webhely helyét egy másik webhelyre az eredeti webhely archiválása közben. A csoportwebhelyhez (csoporthoz nincs kapcsolva) és a kommunikációs webhelyhez is elérhető.

**Fontos:** Ne törölje a klasszikus gyökérwebhelyet modern kommunikációs webhely létrehozásához. Ezt a Microsoft nem támogatja. A gyökérwebhely törlésével a szervezet összes SharePoint elérhetetlenné teszi az összes felhasználó számára, amíg nem visszaállítja a webhelyet, vagy nem hoz létre új webhelyet ugyanazon AZ URL-címen. Ezt a funkciót az üzenetközponton keresztül fogjuk tudatni. Számíthat rá, hogy hamarosan be lesz kapcsolva a szolgáltatás a bérlői webhelyen.

## <a name="known-issues-with-swapping-sites"></a>Ismert problémák a webhelyek felcserélésével
- Előfordulhat, hogy a célwebhely rövid ideig "nem található" (HTTP 404) hibát ad vissza.
- A keresési index frissítéséhez a tartalmat vissza kell tolni. Itt nincs szükség manuális lépésre, ez automatikusan megtörténik.
- A statikus hivatkozásoktól (például Fájlszinkronizálás és OneNote) függő összes adatokat manuálisan kell kijavítani.
- Project Előfordulhat, hogy ellenőrizni kell a kiszolgálói webhelyeket annak érdekében, hogy a megfelelő módon legyen társítva. 
