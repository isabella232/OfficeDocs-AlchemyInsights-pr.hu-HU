---
title: Swap a Classic root oldalon egy modern site
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749262"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap a Classic root oldalon egy modern site

Ha a környezet beállítása április 2019 előtt történt, akkor a Microsoft PowerShell eszközzel megváltoztathatja a gyökérwebhelyet egy modern webhelyre:

- Ha más webhely van, amelyet gyökérwebhelyként kíván használni, kicserélheti [a gyökérwebhelyet](https://docs.microsoft.com/sharepoint/modern-root-site) vele. 
    - Az [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) használata segítségével kicserélheti egy webhely helyét egy másik webhelyre az eredeti webhely archiválása közben. Elérhető mindkét csoportwebhelyhez (nem kapcsolódik csoporthoz) és kommunikációs webhelyhez. 

- A további képességek hamarosan bevezetésre kerülnek, amely lehetővé teszi, hogy folyamatosan használja a tartalmat az oldalon, de átalakítani a meglévő webhely kommunikációs site. 
>[!Important]
>Ezek képességek lesz összecsavart ki fokozatosan. A frissítésekért folytassa az Office 365 Message Center ellenőrzését. 

## <a name="known-issues-with-swapping-sites"></a>A helyek swapping ismert problémái

- A célwebhely rövid ideig "nem található" (HTTP 404) hibát ad vissza.
- A keresési index frissítéséhez a tartalmat recrawled kell. Manuális lépésekre nincs szükség-ezt automatikusan elvégzi.
- A "statikus" hivatkozásokra (például a fájlszinkronizálás és a OneNote-fájlok) vonatkozó bármit manuálisan kell javítani.
- Ha a forráswebhely egy szervezeti hírwebhely volt, frissítse az URL-címet.Kap egy listát az összes szervezeti híroldalak.
- Előfordulhat, hogy a Project Server webhelyeit érvényesíteni kell annak érdekében, hogy még mindig helyesen legyenek társítva.





