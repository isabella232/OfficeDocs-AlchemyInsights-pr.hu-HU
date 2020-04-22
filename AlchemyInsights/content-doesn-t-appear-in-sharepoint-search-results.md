---
title: A tartalom nem jelenik meg a SharePoint keresési eredményei között
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705663"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>A tartalom nem jelenik meg a SharePoint keresési eredményei között

Kövesse az alábbi hibaelhárítási lépéseket, ha a várt tartalom nem jelenik meg a keresési eredmények között:
  
1. Ellenőrizze, hogy a várt tartalmat tartalmazó **webhely** úgy van-e beállítva, hogy a tartalom megjelenjen a keresési eredmények között. Kövesse a [Tartalom megjelenítése a webhelyen](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)a keresési eredmények között című részben leírt lépéseket.

2. Ellenőrizze, hogy a várt tartalmat tartalmazó **lista** vagy **tár** úgy van-e beállítva, hogy a tartalom megjelenjen a keresési eredmények között. Kövesse a [Tartalom megjelenítése listákból vagy tárakból](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)a keresési eredmények között című részben leírt lépéseket.

3. Ellenőrizze, hogy az oldal, a dokumentum vagy az egyéni lapelrendezés **főverzióként van-e közzétéve.** Kövesse a [Keresés](https://go.microsoft.com/fwlink/?linkid=874525)3.

4. Ellenőrizze, hogy a felhasználó **rendelkezik-e engedéllyel** a tartalom megtekintéséhez. Kövesse a [SharePoint engedélyszintek ismertsék el ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels)című témakör lépéseit.
    
5. Ha a keresési sémát új felügyelt tulajdonság hozzáadásával, felügyelt tulajdonság szerkesztésével vagy egy felügyelt tulajdonság eltávolításával módosították, akkor bejárást és újraindexelést kell kérnie. A tartalom **újbóli indexelése** a [Webhely, tár vagy lista bejárásának és újraindexelésének kézi kérése című lépéslépéseit követve.](https://docs.microsoft.com/sharepoint/crawl-site-content) Ez eltarthat egy ideig, várjon 24 órát, mielőtt újra ellenőrizné az eredményeket.

További információt a Tartalom keresése a webhelyen című [témakörben talál.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
