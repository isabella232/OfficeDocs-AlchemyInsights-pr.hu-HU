---
title: Hiányzó munkafolyamat aktiválása sikertelen
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473045"
---
# <a name="missing-workflow-failed-to-activate"></a>Hiányzó munkafolyamat aktiválása sikertelen

A Microsoft SharePoint-webhelycsoport nem adhat (például a "Jóváhagyás – SharePoint 2010") globálisan újrafelhasználható munkafolyamat listához vagy könyvtárhoz.
  
A probléma megoldásához kövesse az alábbi lépéseket: 
  
1. Nyissa meg a legfelső szintű webhely helycsoport a SharePoint Designer 2013.
  
2. **A helyobjektumok**jelölje be a **munkafolyamatok**. 
  
3. A **munkafolyamatok** menüszalag **Új** csoportjában jelölje be **Újrahasználható munkafolyamat**. 
  
4. Az **Újrahasználható munkafolyamat létrehozása** űrlapon adja meg a nevét ** *Repair2010* **. **Platform típusát**kattintson a **SharePoint 2010 munkafolyamat**, és kattintson az **OK gombra**. 
  
1. A **munkafolyamat** -menüszalag **mentése** csoportjában jelölje be **a közzététel**. 
  
2. A **munkafolyamat** -menüszalag **kezelése** csoportjában válassza **Globálisan közzétenni**. A megjelenő megerősítést kérő párbeszédpanelen kattintson az **OK gombra**. 
  
3. Egy webböngészőben keresse meg a legfelső szintű webhely helycsoport, és hozzáférhet a **Webhely beállításai** \> **Webhelycsoport-szolgáltatások**. A **munkafolyamat** -szolgáltatás ezután váltása: 
  
· Ha a szolgáltatás *aktív* , kattintson az **Inaktiválás,** és kattintson az **Aktiválás**. 
  
· Ha a szolgáltatás *inaktívvá válnak* , kattintson az **Aktiválás**. 
  
További információt találhat a következő [cikk](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

