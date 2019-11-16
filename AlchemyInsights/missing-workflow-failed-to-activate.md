---
title: Hiányzó munkafolyamat-aktiválás nem sikerült
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "36753798"
---
# <a name="missing-workflow-failed-to-activate"></a>Hiányzó munkafolyamat-aktiválás nem sikerült

Microsoft SharePoint-webhelycsoportban listához vagy tárhoz nem adhat globálisan újrafelhasználható munkafolyamatot (például "jóváhagyás-SharePoint 2010").
  
A probléma megoldásához hajtsa végre az alábbi lépéseket: 
  
1. Nyissa meg a webhelycsoport gyökérwebhelyét a SharePoint Designer 2013 alkalmazásban.
  
2. A **Webhelyobjektumok**területen válassza a **munkafolyamatok**témakört. 
  
3. A **munkafolyamat** -szalag **új** szakaszában válassza az **újból felhasználható munkafolyamat**-t. 
  
4. Az **újrahasználható munkafolyamat létrehozása** űrlapon adja meg a * * *Repair2010* * * nevet. A **Platformtípus**lapon kattintson a **SharePoint 2010 munkafolyamat**elemre, majd kattintson **az OK gombra**. 
  
1. A **munkafolyamat** -szalag **Mentés** szakaszában válassza a **Közzététel**. 
  
2. A **munkafolyamat** menüszalagjának **kezelés** szakaszában jelölje ki a **globálisan közzéteszi**választógombot. A megerősítést kérő párbeszédpanelen kattintson az **OK gombra**. 
  
3. A webböngészőben keresse meg a webhelycsoport gyökérwebhelyét, és kattintson a **webhelybeállítások** \> webhelycsoport- **szolgáltatásainak**elérésére. Majd a **munkafolyamatok** funkció váltása: 
  
· Ha a szolgáltatás *aktiválva* van, kattintson az **inaktiválás elemre,** majd kattintson az **aktiválás**lehetőségre. 
  
· Ha a szolgáltatás *inaktív* , kattintson az **aktiválás**gombra. 
  
További információért olvassa el a következő [cikket](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

