---
title: Hozzáférés megtagadva üzenetek hibaelhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690785"
---
# <a name="troubleshoot-access-denied-messages"></a>Hozzáférés megtagadva üzenetek hibaelhárítása

Ha valaki "hozzáférés megtagadva" üzenetet kapott egy megosztott mappához a SharePointban, előfordulhat, hogy a webhelycsoport rendszergazdája engedélyezte a "korlátozott hozzáférésű felhasználói engedély zárolási üzemmódját" jelölőnégyzetet. A funkció kikapcsolása: 
  
1. Tallózással keresse meg a webhelyet, kattintson a Beállítások ikonra, majd a **webhely beállításai**parancsra.
    
2. A webhelycsoport **felügyelete**csoportban kattintson a webhelycsoport **szolgáltatásai**hivatkozásra.
    
3. A **korlátozott hozzáférésű felhasználói engedély zárolási üzemmódja**mellett kattintson az **inaktiválás**gombra.
    
Ha a webhely közzétételi webhelye, a megosztott mappákhoz hozzáférés-megtagadási üzenet is előfordulhat. További információ: [hozzáférés megtagadva egy megosztott mappa elérésekor](https://go.microsoft.com/fwlink/?linkid=2004317).
  
Ha valaki "hozzáférés megtagadva" üzenetet kapott a hozzáférési kérelmek megtekintésekor, a felhasználót a webhelycsoport rendszergazdája vagy a webhely tulajdonosok csoportjának tagjaként kell hozzáadnia. További információt a [hozzáférés megtagadva a hozzáférési kérelmek listájához](https://go.microsoft.com/fwlink/?linkid=2004220)című témakörben talál.
  
Ha egy felhasználó "hozzáférés megtagadva" üzenetet kapott, miután eltávolítottak őket a helyszíni Active Directoryból, majd újból hozzáadta őket, tekintse át a [hozzáférés megtagadva, ha a felhasználói fiók szinkronizálva van a Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318)-val.
  

