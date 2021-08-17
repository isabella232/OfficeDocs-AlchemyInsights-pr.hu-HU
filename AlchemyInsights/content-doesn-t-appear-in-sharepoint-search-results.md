---
title: A tartalom nem jelenik meg a SharePoint találatok között
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081612"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>A tartalom nem jelenik meg a SharePoint találatok között

Kövesse az alábbi hibaelhárítási lépéseket, ha a várt tartalom nem jelenik meg a keresési eredményekben:
  
1. Ellenőrizze, hogy **a várt** tartalmat tartalmazó webhely úgy van-e beállítva, hogy a tartalom megjelenjen a keresési eredményekben. Kövesse a Tartalom megjelenítése [a webhelyen a keresési eredményekben lépésre.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)

2. Ellenőrizze, hogy  **a** várt tartalmat tartalmazó lista vagy tár úgy van-e beállítva, hogy a tartalom megjelenjen a keresési eredményekben. Kövesse a Tartalom megjelenítése listákból vagy tárakból a [keresési eredményekben lépésre.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. Ellenőrizze, hogy a lap, dokumentum vagy egyéni lapelrendezés főverzióként **van-e közzétéve.** Kövesse a 3. lépést a Keresés nem adja vissza az összes találatot az [SharePoint keresésben.](https://go.microsoft.com/fwlink/?linkid=874525)

4. Ellenőrizze, hogy a felhasználó rendelkezik-e **a** tartalom megtekintésére vonatkozó engedélyekkel. Kövesse A hozzáférés jogosultsági [szintjeinek](https://docs.microsoft.com/sharepoint/understanding-permission-levels)ismertetése SharePoint.
    
5. Ha a keresési séma módosult egy új felügyelt tulajdonság hozzáadásával, egy felügyelt tulajdonság szerkesztésével vagy egy felügyelt tulajdonság eltávolításával, akkor bejárási és újraindexelési kérésre van szükség. **A webhely,** tár vagy lista bejárási és újraindexelésének manuális kérése lépéseit követve indexelheti [újra a tartalmat.](https://docs.microsoft.com/sharepoint/crawl-site-content) Ez egy kis ideig is eltelhet, és várjon 24 órát, mielőtt ismét ellenőrizi az eredményeket.

További információ: [Keresés](https://docs.microsoft.com/sharepoint/make-site-content-searchable)engedélyezése egy webhelyen. 
  
