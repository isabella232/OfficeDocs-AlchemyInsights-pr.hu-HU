---
title: Teljesítménnyel kapcsolatos problémák – SharePoint vagy OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771903"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>A SharePoint és a OneDrive lassú, elérhetetlen vagy nem érhető el egyszerre több felhasználó esetében

Előfordulhat, hogy a SharePoint vagy a OneDrive lassú, elérhetetlen vagy elérhetetlen, vagy a szolgáltatás nem érhető el, vagy a 503 hibája, több okból kifolyólag:
  
- Ha SharePoint-vagy OneDrive-webhelye lassú vagy késleltetett több felhasználó esetében, előfordulhat, hogy ideiglenes szolgáltatási probléma merül fel, ahol a felhasználók időnként késleltetve vagy navigációs hibákba ütköznek a SharePoint-webhelyek vagy a OneDrive-tartalmak elérésekor. A [szolgáltatás állapota irányítópulton](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) ellenőrizheti, hogy a szervezete hatással van-e rá.
  
- A felhasználók a SharePoint-vagy a OneDrive-webhelyeken való navigáláskor elfoglalt hibába ütközhet a *503-kiszolgálóval* . Ezt a hibát a SharePoint-szolgáltatáson belüli szabályozás okozhatja. A SharePoint Online a szabályozást használja a SharePoint Online szolgáltatás optimális teljesítményének és megbízhatóságának fenntartásához. A szabályozás korlátozza a felhasználói műveletek vagy a párhuzamos hívások számát (parancsprogrammal vagy kóddal) az erőforrások túlzott felhasználásának megelőzése érdekében. A szabályozással kapcsolatos további tudnivalókért olvassa el a [SharePoint Online-ban a letiltott vagy Letiltva](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)jelölőnégyzetet.

- Ha gyenge teljesítményt tapasztal egy **klasszikus** vagy **modern** SharePoint-webhelyen vagy-lapon, használja a [lap diagnosztikai eszközét](https://aka.ms/perftool) a lapok elemzéséhez.
  
- Ha továbbra is általános gyenge teljesítményt tapasztal, olvassa el a jelen cikk alján található forrásokat: [Bevezetés a SharePoint Online teljesítményének finomhangolásával](https://go.microsoft.com/fwlink/?linkid=2024334)
  