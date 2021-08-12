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
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940821"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>A klasszikus gyökérwebhely felcserélizálása modern webhelyekkel

Ha a környezete 2019 áprilisa előtt volt beállítva, a Microsoft PowerShell segítségével modern webhelyre módosíthatja a gyökérwebhelyet:

- Ha van egy másik webhelye, amit gyökérwebhelyként szeretne használni, helyettesítheti [(felcserélheti)](https://docs.microsoft.com/sharepoint/modern-root-site) a gyökérwebhelyet vele. 
    - Az [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) segítségével felcserélje egy webhely helyét egy másik webhelyre az eredeti webhely archiválásával. A csoportwebhely (csoporthoz nem kapcsolt) és a kommunikációs webhely számára is elérhető. 

- Hamarosan további funkciókat is bevezetünk, amelyek lehetővé teszik, hogy továbbra is a webhelyen lévő tartalmakat használja, de a meglévő webhelyet kommunikációs webhelyké alakítsa át. 
>[!Important]
>Ezeket a képességeket fokozatosan vezetjük be. Folytassa a frissítéseket az Üzenetközpontban. 

## <a name="known-issues-with-swapping-sites"></a>Ismert problémák a webhelyek felcserélésével

- Előfordulhat, hogy a célwebhely rövid ideig "nem található" (HTTP 404) hibát ad vissza.
- A keresési index frissítéséhez a tartalmat vissza kell tolni. Nincs szükség manuális lépésre – ez automatikusan történik.
- A statikus hivatkozásoktól (például Fájlszinkronizálás és OneNote) függő összes adatokat manuálisan kell kijavítani.
- Ha a forráswebhely szervezeti hírwebhely volt, frissítse az URL-címet. Az összes szervezeti híroldal listájának lekérte.
- Project Előfordulhat, hogy ellenőrizni kell a kiszolgálói webhelyeket annak érdekében, hogy a megfelelő módon legyen társítva.
