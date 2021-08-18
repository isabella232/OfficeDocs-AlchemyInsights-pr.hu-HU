---
title: A Megnyitás Intézővel programmal kapcsolatos hibák elhárítása
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323568"
---
# <a name="fix-problems-with-open-with-explorer"></a>A Megnyitás Intézővel programmal kapcsolatos problémák elhárítása

A Megnyitás Intézővel paranccsal megoldhatja a dokumentumtárak megnyitásakor SharePoint vagy OneDrive **problémákat:** 
  
- Használja Internet Explorer 10 az Internet Explorer 11-et. **A Megnyitás Intézővel** nem kompatibilis a Microsoft Edge, a Google Chrome, a Firefox és más böngészők használatával. **A Megnyitás Intézővel gombra** az Internet Explorer kivételével minden böngészőben le van tiltva. 
    
- **A Megnyitás Intézővel** lehetőség a dokumentumtárak modern felhasználói SharePoint érhető el. Használja **inkább a Nézet a Fájlkezelőben ehelyett.** Válassza **a Nézetbeállítások Nézet** a \> **Fájlkezelőben lehetőséget.** A Megtekintés a Fájlkezelőben nem kompatibilis a Microsoft Edge, a Google Chrome, a Firefox és más felhasználókkal. **A Megtekintés a Fájlkezelőben csak** az Internet Explorerben érhető el. 
    
- Ellenőrizze, hogy fut-e a WebClient szolgáltatás. A Windows írja be a futtatás parancsot, válassza az Asztali futtatás alkalmazást, írja be a services.msc parancsot, és nyomja le az Enter billentyűt. Görgessen le a WebClient szolgáltatáshoz, és győződjön meg arról, hogy az **Állapot oszlopban** a "Fut" szó látható. Ha nem így van, kattintson duplán a szolgáltatásra, kattintson a **Start gombra,** majd az **OK gombra.** (Lehetséges, hogy előbb engedélyeznie kell  a  szolgáltatást az Indítási típus mező Kézi vagy Automatikus **beállításával.)** 
    
**Megjegyzés:** Akkor érdemes a Fájlkezelőben megnyitni egy tárat, ha egyszerre több fájlt és mappát kell másolnia vagy áthelyezni, de ha rendszeresen szeretne dolgozni a tárban, azt javasoljuk, hogy szinkronizálja. A Fájlkezelőben való megnyitással kapcsolatos hibák elhárításához tekintse meg a Megnyitás [Intézőben témakört.](https://go.microsoft.com/fwlink/?linkid=871665) A szinkronizálás beállításával kapcsolatos további információkért lásd: SharePoint fájlok szinkronizálása az új OneDrive szinkronizálási app [ügyfélalkalmazással.](https://go.microsoft.com/fwlink/?linkid=871666)
  
További információért olvassa el A Megnyitás Intézővel parancs használata a SharePoint [hibák](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) elhárításához. 
  

