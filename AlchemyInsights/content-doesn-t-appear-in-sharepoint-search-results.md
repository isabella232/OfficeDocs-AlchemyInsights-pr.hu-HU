---
title: Tartalom nem jelenik meg a SharePoint-találatok
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517033"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Tartalom nem jelenik meg a SharePoint-találatok

Hajtsa végre az alábbi lépéseket, ha a várt tartalom nem jelenik meg a keresési eredmények között:
  
1. Ellenőrizze, hogy a várt tartalom tartalmazó **webhely** beállításai lehetővé teszik a tartalom jelenjen meg a keresési eredmények között. Kövesse [a keresési eredmények között a webhely tartalmának megjelenítése](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Ellenőrizze, hogy a **lista** vagy **dokumentumtár** , amely tartalmazza a várt tartalom beállításai lehetővé teszik a tartalom jelenjen meg a keresési eredmények között. Kövesse a [listák vagy tárak a keresési eredmények között a tartalom megjelenítése](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Ellenőrizze, hogy a lap, dokumentum vagy egyéni lap elrendezése is közzétételre kerülnek a **főverzió.** Hajtsa végre a 3 a [Keresés nem ad vissza a SharePoint Online összes eredmény](https://go.microsoft.com/fwlink/?linkid=874525).

4. Győződjön meg arról, hogy a felhasználó rendelkezik-e **engedéllyel** a tartalom megtekintését. Kövesse a [SharePoint jogosultsági szintek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Ha a Keresés séma megváltozott, egy új felügyelt tulajdonság hozzáadása, felügyelt tulajdonság szerkesztése, vagy egy kezelt tulajdonságnak, majd a bejárás kérő eltávolításával és újraindexeli lesz szükség. **Újraindexelni** a tartalmat [kézzel a bejárási és indexelési újra a hely, a tár vagy lista kérése](https://docs.microsoft.com/sharepoint/crawl-site-content)utasításait követve. Ez lehet, hogy hosszabb ideig eltarthat, Várjon 24 órát az eredmények ismételt ellenőrzés előtt.

További tudnivalókért tanulmányozza [a helyszínen kell kereshető tartalom engedélyezése](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
