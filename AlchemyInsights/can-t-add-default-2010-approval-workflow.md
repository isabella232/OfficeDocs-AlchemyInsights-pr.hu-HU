---
title: Nem lehet hozzáadni az alapértelmezett jóváhagyási munkafolyamat 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293068"
---
# <a name="cant-add-default-2010-approval-workflow"></a>Nem lehet hozzáadni az alapértelmezett jóváhagyási munkafolyamat 2010

A Microsoft SharePoint-webhelycsoport nem adhat (például a "Jóváhagyás – SharePoint 2010") globálisan újrafelhasználható munkafolyamat listához vagy könyvtárhoz.
  
A probléma megoldásához kövesse az alábbi lépéseket: 
  
1. Nyissa meg a legfelső szintű webhely helycsoport a SharePoint Designer 2013.
  
2. **A helyobjektumok**jelölje be a **munkafolyamatok**. 
  
3. A **munkafolyamatok** menüszalag **Új** csoportjában jelölje be **Újrahasználható munkafolyamat**. 
  
4. Az **Újrahasználható munkafolyamat létrehozása** űrlapon adja meg nevét * **Repair2010***. **Platform típusa**jelölje be a **SharePoint 2010 munkafolyamat**, és kattintson az **OK gombra**. 
  
5. A **munkafolyamat** -menüszalag **mentése** csoportjában jelölje be **a közzététel**. 
  
6. A **munkafolyamat** -menüszalag **kezelése** csoportjában válassza **Globálisan közzétenni**. A megjelenő megerősítést kérő párbeszédpanelen kattintson az **OK gombra**. 
  
7. Egy webböngészőben keresse meg a legfelső szintű webhely helycsoport, és hozzáférhet a **Webhely beállításai** \> **Webhelycsoport-szolgáltatások**. A **munkafolyamat** -szolgáltatás ezután váltása: 
  
· Ha a szolgáltatás *aktív* , kattintson az **Inaktiválás,** és kattintson az **Aktiválás**. 
  
· Ha a szolgáltatás *inaktívvá válnak* , kattintson az **Aktiválás**. 
  
További információt találhat a következő [cikk](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

