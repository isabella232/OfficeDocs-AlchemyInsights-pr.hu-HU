---
title: A SharePoint Online keresés
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507633"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>A bejárási és indexelési a SharePoint Online tartalom

Tartalom bejárása legyen, és hozzáadódnak a keresési index számára, hogy mi azok keres a SharePoint Online keresése. Automatikusan a bejárt tartalmat alapján előre definiált bejárási ütemezés (a bejárás ütemezése nem lehet módosítani). A webbejáró veszi fel tartalmat, amely a legutóbbi bejárás óta megváltozott, és frissíti az indexet. A bejárt tartalmat, és az index frissítése érdekében vegye figyelembe az alábbiakat:

- Ellenőrizze, hogy azáltal, [hogy a webhely tartalma kereshető](https://docs.microsoft.com/sharepoint/make-site-content-searchable)tartalom található.

- Felügyelt tulajdonság módosítása után, vagy ha megváltoztatta hozzárendelése bejárt és kezelt tulajdonságai, a webhely bejárását előtt kell a változások megjelennek a keresési indexben. 

    A módosítások megjelennek a keresési sémában, és nem a tényleges hely, mert a webbejáró nem automatikusan újra indexeli a webhelyet. 

    További információért lásd: [manuálisan kérheti a bejárási és indexelési újra a hely, a tár vagy lista](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Várjon, amíg manuálisan a bejárás és teljes újraindexelése megtekintéséhez, ha még mindig fennáll a probléma bekérése után legalább 24 órán keresztül. 

    Ha 24 óránál hosszabb idő telt el azóta a bejárás és a teljes újraindexelése kezdeményezett, jelentkezzen be a támogatási eset. Sok esetben azt már dolgozik a megoldáson. Adja meg a megoldás végrehajtásához legalább 24 órán keresztül.

> [!IMPORTANT]
> Ha egy webhely (könyvtár) a dokumentum vagy lista törölve lett, és még mindig szerepel a keresési eredmények a felhasználók kell kapnia egy **Hiba 404 fájl nem található** az elérésére tett kísérlet során. A probléma további vizsgálatához támogatási eset kell naplózásra. 



