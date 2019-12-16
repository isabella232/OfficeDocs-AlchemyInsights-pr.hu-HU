---
title: Nem lehet hozzáadni a 2010 jóváhagyási munkafolyamatot
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049555"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Nem lehet hozzáadni a 2010 jóváhagyási munkafolyamatot

Microsoft SharePoint-webhelycsoportban listához vagy tárhoz nem adhat globálisan újrafelhasználható munkafolyamatot (például "jóváhagyás-SharePoint 2010").
  
A probléma megoldásához hajtsa végre az alábbi lépéseket: 
  
1. Nyissa meg a webhelycsoport gyökérwebhelyét a SharePoint Designer 2013 alkalmazásban.
  
2. A **Webhelyobjektumok**területen válassza a **munkafolyamatok**témakört. 
  
3. A **munkafolyamat** -szalag **új** szakaszában válassza az **újból felhasználható munkafolyamat**-t. 
  
4. Az **újrahasználható munkafolyamat létrehozása** űrlapon adja meg a * * *Repair2010* * * nevet. A **Platformtípus**lapon kattintson a **SharePoint 2010 munkafolyamat**elemre, majd kattintson **az OK gombra**. 
  
1. A **munkafolyamat** -szalag **Mentés** szakaszában válassza a **Közzététel**. 
  
2. A **munkafolyamat** menüszalagjának **kezelés** szakaszában jelölje ki a **globálisan közzéteszi**választógombot. A megerősítést kérő párbeszédpanelen kattintson az **OK gombra**. 
  
3. A webböngészőben keresse meg a webhelycsoport gyökérwebhelyét, és kattintson a **webhelybeállítások** \> webhelycsoport- **szolgáltatásainak**elérésére. A **munkafolyamatok** funkció váltása: 
  
· Ha a szolgáltatás *aktiválva* van, kattintson az **inaktiválás elemre,** majd kattintson az **aktiválás**lehetőségre. 
  
· Ha a szolgáltatás *inaktív* , kattintson az **aktiválás**gombra. 
  
További információért olvassa el a következő [cikket](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

