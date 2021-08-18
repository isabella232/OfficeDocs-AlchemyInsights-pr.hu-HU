---
title: A klasszikus gyökérwebhely felcserélizálása modern webhelyekkel
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316142"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>A klasszikus gyökérwebhely felcserélizálása modern webhelyekkel

Ha a környezetét 2019 áprilisa előtt beállította, a gyökérwebhelyet modern webhelyre módosíthatja a Microsoft PowerShell használatával:

- Ha van egy másik webhelye, amit gyökérwebhelyként szeretne használni, helyettesítheti [(felcserélheti)](https://docs.microsoft.com/sharepoint/modern-root-site) a gyökérwebhelyet vele. 
    - Az [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) használatával felcserélje egy webhely helyét egy másik webhelyre az eredeti webhely archiválása közben. A csoportwebhelyhez (csoporthoz nincs kapcsolva) és a kommunikációs webhelyhez is elérhető. 

- Hamarosan további funkciókat is bevezetünk, amelyek lehetővé teszik, hogy továbbra is a webhelyen lévő tartalmakat használja, de a meglévő webhelyet kommunikációs webhelyké alakítsa át. 

**Fontos:** Ezeket a képességeket fokozatosan vezetjük be. Folytassa a frissítéseket az Üzenetközpontban. 

## <a name="known-issues-with-swapping-sites"></a>Ismert problémák a webhelyek felcserélésével

- Előfordulhat, hogy a célwebhely rövid ideig "nem található" (HTTP 404) hibát ad vissza.
- A keresési index frissítéséhez a tartalmat vissza kell tolni. Nincs szükség manuális lépésre – ez automatikusan történik.
- A statikus hivatkozásoktól (például Fájlszinkronizálás és OneNote) függő összes adatokat manuálisan kell kijavítani.
- Ha a forráswebhely szervezeti hírwebhely volt, frissítse az URL-címet. Az összes szervezeti híroldal listájának lekérte.
- Project Előfordulhat, hogy ellenőrizni kell a kiszolgálói webhelyeket annak érdekében, hogy a megfelelő módon legyen társítva.
