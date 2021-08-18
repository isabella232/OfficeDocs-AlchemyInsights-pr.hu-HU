---
title: A Megnyitás Intézővel nem működik
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321863"
---
# <a name="open-with-explorer-isnt-working"></a>Nem működik a Megnyitás Intézővel

Ha **a Megnyitás Intézővel vagy** a Megtekintés a Fájlkezelőben beállítás  nem működik, ellenőrizze, hogy a WebClient szolgáltatás Futás beállítására van-e állítva az alábbi lépéseket követve.  Hosszú ideig is tart például egy SharePoint vagy OneDrive tár megnyitása, amikor a szolgáltatás nem fut. 
  
1. A Windows írja be a futtatás parancsot, válassza az Asztali futtatás alkalmazást, írja be a services.msc parancsot, majd válassza az **Enter lehetőséget.**
    
2. Görgessen le a WebClient szolgáltatáshoz, és ellenőrizze az **Állapot oszlopot.** Ha a WebClient szolgáltatás állapota nem **Fut,** kattintson duplán a szolgáltatásra, kattintson a **Start** gombra, majd az **OK gombra.** Szükség esetén engedélyezze a szolgáltatást  az  Indítási típus mező Kézi vagy Automatikus **beállításával.** 
    
**Megjegyzés:** A Fájlkezelőben való megnyitással kapcsolatos hibák elhárításához tekintse meg a Megnyitás [Intézővel témakört.](https://go.microsoft.com/fwlink/?linkid=871665) Ismerje meg a szinkronizálást jobb alternatívaként: Szinkronizálja a SharePoint az új ügyfélalkalmazással [OneDrive szinkronizálási app fájlokat.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

