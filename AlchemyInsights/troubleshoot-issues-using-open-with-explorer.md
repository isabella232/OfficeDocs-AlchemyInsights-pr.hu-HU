---
title: A Megnyitás intézővel című programmal kapcsolatos problémák elhárítása
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759694"
---
# <a name="fix-problems-with-open-with-explorer"></a>Az Open with Explorer programmal kapcsolatos problémák megoldása

Javítsa ki a SharePoint vagy a OneDrive dokumentumtárának megnyitásával kapcsolatos gyakori problémákat a **Megnyitás az Intézővel** paranccsal: 
  
- Használja az Internet Explorer 10-et vagy az Internet Explorer 11-et. **A Open with Explorer** nem kompatibilis a Microsoft Edge, a Google Chrome, a Firefox és mások alkalmazásával. **Az Intézővel megnyitva** minden böngészőben le van tiltva, kivéve az Internet Explorert. 
    
- **A Nyitott az Intézővel** program nem érhető el a SharePoint-tárak modern élményében. Használja inkább **a Nézet a Fájlkezelőben** lehetőséget. Válassza **a Nézet lehetőséget** \> **a Fájlkezelőben**. View in File Explorer nem kompatibilis a Microsoft Edge, a Google Chrome, a Firefox és mások. **A Fájlkezelőben** csak az Internet Explorer ben érhető el. 
    
- Ellenőrizze, hogy fut-e a WebClient szolgáltatás. A Windows keresőmezőjében írja be a futtatás t, jelölje be az Asztali alkalmazás futtatása jelölőnégyzetet, írja be a services.msc parancsot, majd nyomja le az Enter billentyűt. Görgessen le a WebClient szolgáltatáshoz, és győződjön meg arról, hogy az **Állapot** oszlopban a "Futás" látható. Ha nem, kattintson duplán a szolgáltatásra, kattintson a **Start**gombra, majd az **OK**gombra. (Előfordulhat, hogy először engedélyeznie kell a szolgáltatást, ha az **Indítás típusa** mezőben a **Kézi** vagy az **Automatikus** lehetőséget választja.) 
    
> [!NOTE]
> A Fájlkezelőben megnyitegy tárat, ha egyszer több fájlt és mappát kell másolnia vagy áthelyeznie, de ha rendszeresen szeretne dolgozni a tárban, javasoljuk, hogy szinkronizálja azt. A Fájlkezelőben megnyitott problémák elhárításáról a [Megnyitás az Intézőben című témakörben](https://go.microsoft.com/fwlink/?linkid=871665)található. A szinkronizálás beállításáról a [SharePoint-fájlok szinkronizálása az új OneDrive szinkronizálási ügyfélalkalmazással](https://go.microsoft.com/fwlink/?linkid=871666)című témakörben talál.
  
További információt a ["Megnyitás explorerrel" paranccsal a SharePoint Online-ban felmerülő problémák elhárítására](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) című cikkben talál. 
  

