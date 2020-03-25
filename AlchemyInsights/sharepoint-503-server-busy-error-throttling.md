---
title: SharePoint Online szabályozása
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931228"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online szabályozása

**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben. Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások. Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.

Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon. Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben. Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.

**Az 503-as kiszolgáló foglalt hiba**

Előfordulhat, hogy a felhasználók 503-as kiszolgálófoglalt hibaüzenetet kapnak, amikor SharePoint- vagy OneDrive-webhelyekre próbálnak navigálni. 

Ezt a hibát a SharePoint szolgáltatáson belüli szabályozás okozhatja. A SharePoint Online szabályozással állítja fenn a SharePoint Online-szolgáltatás optimális teljesítményét és megbízhatóságát. Szabályozás korlátozza a felhasználói műveletek számát vagy egyidejű hívások (parancsfájl vagy kód) az erőforrások túlzott használatának megelőzése érdekében. 

A szabályozásról további információt a [SharePoint Online-ban található Szabályozás elkerülése című témakörben](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)talál.

Ha úgy véli, hogy ez a hiba nem kapcsolódik a szabályozáshoz, ellenőrizheti, hogy a bérlőn aktív karbantartás történik-e, ha az [Üzenetközpontra](https://portal.office.com/adminportal/home#/MessageCenter)navigál.

 Végül győződjön meg róla, hogy látogasson el a [Service Health](https://portal.office.com/adminportal/home#/servicehealth) oldalra, hogy ellenőrizze az esetlegesen előforduló tanácsokat/incidenseket.

