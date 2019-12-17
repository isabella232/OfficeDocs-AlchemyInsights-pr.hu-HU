---
title: Teljesítménnyel kapcsolatos problémák-SharePoint vagy OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068406"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>A SharePoint vagy az OneDrive lassú, elérhetetlen vagy nem érhető el több felhasználó számára

A SharePoint vagy az OneDrive lelassulhat, hozzáférhetetlen vagy nem érhető el, és több okból is elérhetetlenné vagy 503 hibát okozhat:
  
- Ha a SharePoint vagy az OneDrive webhelye lassú, vagy több felhasználó számára késik, előfordulhat, hogy átmeneti szolgáltatási probléma áll fenn, ahol a felhasználók a SharePoint-webhelyek vagy az OneDrive-tartalom elérése közben időszakos késleltetést vagy navigációs hibákat tapasztalnak. Ellenőrizze a [szolgáltatás állapotirányítópultját](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , hogy a szervezet érintett-e.
  
- Használók május kap egy *503 szolgál van elfoglalt* hiba mikor kísérlet-hoz hajózik-hozSharepoint vagy OneDrive telek. Ez a hiba a SharePoint-szolgáltatásban történő fojtás esetén is okozhatja. A SharePoint Online az optimális teljesítmény és megbízhatóság fenntartására használja a SharePoint Online szolgáltatást. A fojtás korlátozza a felhasználói műveletek számát vagy az egyidejű hívásokat (parancsfájlokkal vagy kóddal) az erőforrások túlzott használatának megakadályozása érdekében. A szabályozásra vonatkozó további információért [Kerülje a SharePoint Online szolgáltatásban a sávszélesség vagy a Letiltás elkerülését](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Ha a **klasszikus** vagy a **modern** SharePoint-webhellyel vagy-weblapokkal lassú teljesítményt tapasztal, használja az [oldaldiagnosztikai eszközt](https://aka.ms/perftool) az oldalak elemzéséhez.
  
- Ha továbbra is lassú a teljesítmény, tekintse át a cikk alján található forrásokat: [Bevezetés a SharePoint Online teljesítményhangolásához](https://go.microsoft.com/fwlink/?linkid=2024334)
  