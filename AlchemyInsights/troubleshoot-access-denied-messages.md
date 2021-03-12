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
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704896"
---
# <a name="troubleshoot-access-denied-messages"></a>Hozzáférés megtagadva üzenetek hibaelhárítása

Ha valaki "Hozzáférés megtagadva" üzenetet kapott egy Megosztott mappába a SharePointban, előfordulhat, hogy a webhelycsoport rendszergazdája engedélyezte a "Korlátozott hozzáférésű felhasználói engedély zárolási mód" beállítást. A következőt kapcsolhatja ki: 
  
1. Tallózással keresse meg a webhelyet, kattintson a Beállítások ikonra, majd a **Webhely beállításai elemre.**
    
2. A **Webhelycsoport felügyelete alatt kattintson** a **Webhelycsoport-szolgáltatások elemre.**
    
3. A Korlátozott **hozzáférésű felhasználói** engedély zárolási módja mellett kattintson az Inaktiválás **gombra.**
    
A "Hozzáférés megtagadva" üzenet megosztott mappák esetén is előfordulhat, ha a webhely közzétételi webhely. További információért lásd: [Hozzáférés megtagadva megosztott mappa elérésekor.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)
  
Ha valaki "Hozzáférés megtagadva" üzenetet kapott a hozzáférési kérelmek megtekintésekor, a felhasználót fel kell véve webhelycsoport-rendszergazdaként vagy a Tulajdonosok csoport tagjaként a webhelyhez. További információért lásd: Hozzáférés megtagadva a hozzáférési [kérelmek listájához.](https://go.microsoft.com/fwlink/?linkid=2004220)
  
Ha egy felhasználó "Hozzáférés megtagadva" üzenetet kapott, miután eltávolította a helyszíni Active Directoryból, majd hozzáadta őket, a Hozzáférés megtagadva, amikor egy felhasználói fiók szinkronizálódik [a Microsoft 365-be.](https://go.microsoft.com/fwlink/?linkid=2004318)
  

