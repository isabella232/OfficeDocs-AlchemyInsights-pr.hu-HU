---
title: SharePoint áttelepítési szabályozás 503-as hibákkal
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931660"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>SharePoint áttelepítési szabályozás 503-as hibákkal

**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben. Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások. Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.

Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon. Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben. Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.

**503-as hibák a SharePoint Online-ra való áttéréskor**

Úgy tűnik, hogy a SharePoint Online-ra költözik, és 503-as hibákat kap. Kérjük, kövesse az alábbi lépéseket, hogy a lehető leghamarabb segíthessünk Önnek. 

1. Kattintson **a Kapcsolatfelvételi szolgáltatás**, majd **az Új szolgáltatáskérés parancsra.**
2. A cím és a leírás mezőbe írja be a **SharePoint áttelepítési szabályozását az 503-as sal.**
3. A jegy beküldése után kérjük, frissítse a következő információkkal:
    - Mennyi maradt a migrációból (például hány TB?).
    - Áttelepítés kezdő és záró dátuma.
    - Írja le, hogy honnan telepíti át a tartalmat, például a SharePoint Server, a Box, a GDrive, a Fájlmegosztások stb.
    - Becsülje meg a sávszélesség-szabályozási hibák számát (például x sávszélesség-szabályozás óránként?), és mikor történt a szabályozás.
    - Az ön által használt áttelepítési eszköz (például SPMT vagy ShareGate).


