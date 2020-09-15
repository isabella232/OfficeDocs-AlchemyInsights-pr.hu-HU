---
title: A Megnyitás Intézővel parancs használatával kapcsolatos problémák elhárítása
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
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659060"
---
# <a name="fix-problems-with-open-with-explorer"></a>A Megnyitás Intézővel kapcsolatos problémák megoldása

A SharePointban vagy a OneDrive-ban az **Open with Explorer** paranccsal megnyitható gyakori problémák megoldása: 
  
- Használja az Internet Explorer 10 vagy az Internet Explorer 11 alkalmazást. **A Megnyitás Intézővel** nem kompatibilis a Microsoft Edge, a Google Chrome, a Firefox és a többiekkel. A **Megnyitás Intézővel** le van tiltva az összes böngészőben, kivéve az Internet Explorert. 
    
- A **Megnyitás Intézővel** lehetőség nem érhető el a SharePoint-tárak modern felületén. Használja inkább **a nézetet a Fájlkezelőben** . Válassza a **nézet beállításai** \> **nézet lehetőséget a Fájlkezelőben**. A megtekintés a Fájlkezelőben nem kompatibilis a Microsoft Edge, a Google Chrome, a Firefox és a többiekkel. A **fájlkezelőben** csak az Internet Explorerben érhető el nézet. 
    
- Ellenőrizze, hogy fut-e a WebClient szolgáltatás. A Windows Search mezőbe írja be a Futtatás parancsot, és válassza az asztali Futtatás alkalmazást, írja be a Services. msc parancsot, és nyomja le az ENTER billentyűt. Görgessen le a WebClient szolgáltatáshoz, és győződjön meg arról, hogy az **állapot** oszlopban a "Futtatás" szó látható. Ha nem, kattintson duplán a szolgáltatásra, kattintson a **Start**gombra, majd az **OK**gombra. (Előfordulhat, hogy először engedélyeznie kell a szolgáltatást az **indítási típus** mezőben lévő **kézi** vagy **automatikus** elem kiválasztásával.) 
    
> [!NOTE]
> Ha egy tár megnyitása a Fájlkezelőben akkor hasznos, ha egyszerre több fájlt és mappát kell másolni vagy áthelyeznie, de ha rendszeresen dolgozni szeretne a tárban, azt javasoljuk, hogy szinkronizálja. A Fájlkezelőben való megnyitással kapcsolatos hibák elhárításáról a [Megnyitás az Intézőben](https://go.microsoft.com/fwlink/?linkid=871665)című témakörben olvashat. A szinkronizálás beállításáról további információt a [SharePoint-fájlok szinkronizálása az új OneDrive szinkronizálási ügyfélprogrammal](https://go.microsoft.com/fwlink/?linkid=871666)című témakörben talál.
  
További információért olvassa el a [SharePoint Online problémáinak elhárítása című témakört a "Megnyitás Intézővel" paranccsal](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) . 
  

