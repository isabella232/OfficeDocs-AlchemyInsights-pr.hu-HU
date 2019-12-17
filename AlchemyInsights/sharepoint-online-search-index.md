---
title: Keresés a SharePoint Online szolgáltatásban
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044045"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Tartalomfeltérképezés és indexelés a SharePoint Online szolgáltatásban

A tartalmat bejárnia kell, és hozzá kell adnia a keresési indexhez ahhoz, hogy megtalálja a keresést a SharePoint Online szolgáltatásban. A program a tartalmat előre definiált bejárási ütemezés alapján automatikusan feltérképezi (a bejárási ütemezés nem módosítható). A webbejáró felveszi az utolsó bejárás óta módosult tartalmat, és frissíti az indexet. A tartalombejárás és az index frissítése érdekében vegye figyelembe a következőket:

- Győződjön meg arról, hogy tartalma megtalálható a [webhely tartalmának kereshetővé tétele](https://docs.microsoft.com/sharepoint/make-site-content-searchable)érdekében.

- Miután módosította a felügyelt tulajdonságot, vagy módosította a bejárt és kezelt tulajdonságok hozzárendelését, a webhelyet újra kell bejárnia ahhoz, hogy a módosítások megjelenjenek a keresési indexben. 

    Mivel a módosítások a keresési sémában történtek, és nem az aktuális webhelyre, a webbejáró nem fogja automatikusan újra indexelni a webhelyet. 

    További információt a [webhelyek, tárak és listák kézi vagy újraindexelésének manuális kérése](https://docs.microsoft.com/sharepoint/crawl-site-conten)című témakörben talál.

- A bejárás és a teljes újraindex manuális kérése után várjon legalább 24 órát, és ellenőrizze, hogy a probléma továbbra is fennáll-e. 

    Ha több mint 24 óra telt el mióta kezdeményezte a feltérképezés és a teljes re-index, kérjük, jelentkezzen egy támogatási ügyben. Sok esetben már dolgozunk a megoldásban. Kérjük, hogy a megoldás befejezéséhez legalább 24 órát adjon nekünk.

> [!IMPORTANT]
> Ha egy webhelyet, dokumentumot (könyvtárat) vagy listát töröltek, és még mindig láthatók a keresési eredményekben, a felhasználóknak hibaüzenetet kell kapniuk, **404 a fájl nem található** , amikor megpróbálnak hozzáférni hozzá. Ezt a kérdést a további kivizsgálás támogatási eseteként kell naplóznia. 



