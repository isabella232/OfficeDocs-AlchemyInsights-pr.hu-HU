---
title: Hozzáférés megtagadott üzenetekkel kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c62186fd346efd539b13cef9c80f5e797ebf80811a21db73f0f07fd86c080d55
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939885"
---
# <a name="troubleshoot-access-denied-messages"></a>Hozzáférés megtagadott üzenetekkel kapcsolatos hibák elhárítása

Ha valaki "Hozzáférés megtagadva" üzenetet kapott egy megosztott mappába az SharePoint-ban, előfordulhat, hogy a webhelycsoport rendszergazdája engedélyezte a "Korlátozott hozzáférésű felhasználói engedély zárolási módot" beállítást. A kikapcsoláshoz: 
  
1. Tallózással keresse meg a webhelyet, kattintson Gépház ikonra, majd a **Webhelywebhely Gépház.**
    
2. A **Webhelycsoport felügyelete alatt kattintson** a **Webhelycsoport szolgáltatásai elemre.**
    
3. A **Korlátozott hozzáférésű felhasználói** engedély zárolási módja mellett kattintson az Inaktiválás **elemre.**
    
Megosztott mappák esetén a Hozzáférés megtagadva üzenet is bekövetkezhet, ha a webhely egy közzétételi webhely. További információ: [Hozzáférés megtagadva megosztott mappa elérésekor.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)
  
Ha a hozzáférési kérelmek megtekintésekor valaki "Hozzáférés megtagadva" üzenetet kapott, a felhasználót vagy webhelycsoport-rendszergazdaként, vagy a Tulajdonosok csoport tagjaként kell hozzáadni a webhelyhez. További információ: [Hozzáférés megtagadva a hozzáférési kérelmek listájához](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Ha egy felhasználó "Hozzáférés megtagadva" üzenetet kapott, miután eltávolították a helyszíni Active Directoryból, majd újra hozzáadta őket, lásd: Hozzáférés megtagadva, amikor egy felhasználói fiók szinkronizálódik a [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)
  

