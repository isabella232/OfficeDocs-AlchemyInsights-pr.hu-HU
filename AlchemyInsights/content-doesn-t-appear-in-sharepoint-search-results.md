---
title: Nem jelenik meg a tartalom a SharePoint keresési eredményei között
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
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713132"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Nem jelenik meg a tartalom a SharePoint keresési eredményei között

Kövesse ezeket a hibaelhárítási lépéseket, ha a várt tartalom nem jelenik meg a keresési eredmények között:
  
1. Ellenőrizze, hogy a várt tartalmat tartalmazó **webhely** be van-e állítva a tartalom keresési eredményekben való megjelenítésére. Kövesse a [webhely tartalmának megjelenítése a keresési eredményekben](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)című témakör lépéseit.

2. Ellenőrizze, hogy a várt tartalmat tartalmazó **lista** vagy **tár** van-e beállítva, hogy a tartalom a találatok között jelenjen meg. Kövesse a [találatok között a listák vagy tárak tartalmának megjelenítése](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)című témakör lépéseit.

3. Ellenőrizze, hogy a lap, a dokumentum vagy az egyéni lapelrendezés megjelenik-e **fő verzióként.** Kövesse a 3. lépés a [találatok között a SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525)-ban című témakört.

4. Ellenőrizze, hogy a felhasználó rendelkezik-e **engedélyekkel** a tartalom megtekintéséhez. Kövesse a [SharePoint jogosultsági szintjeinek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels)című témakör lépéseit.
    
5. Ha a keresési sémát egy új felügyelt tulajdonság hozzáadásával módosította, a felügyelt tulajdonság szerkesztésével vagy egy felügyelt tulajdonság eltávolításával, majd a bejárási és újraindexelési kéréssel szükséges. **A tartalom újraindexeléséhez** kövesse a [webhely, tár vagy lista bejárásának vagy újraindexelésének manuális kérése című szakasz](https://docs.microsoft.com/sharepoint/crawl-site-content)lépéseit. Ez eltarthat egy darabig, várjon 24 órát, mielőtt ismét ellenőrizni fogja az eredményeket.

További tudnivalókat a [webhelyen kereshető tartalmak engedélyezése](https://docs.microsoft.com/sharepoint/make-site-content-searchable)című témakörben talál. 
  
