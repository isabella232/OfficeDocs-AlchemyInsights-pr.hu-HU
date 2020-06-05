---
title: Nem lehet hozzáadni a 2010-es jóváhagyási munkafolyamatot
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582849"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Nem lehet hozzáadni a 2010-es jóváhagyási munkafolyamatot

Microsoft SharePoint-webhelycsoportban nem adhat hozzá globálisan újrafelhasználható munkafolyamatot (például "Jóváhagyás – SharePoint 2010") listához vagy tárhoz.
  
A probléma megoldásához hajtsa végre az alábbi lépéseket: 
  
1. Nyissa meg a SharePoint Designer 2013 webhelycsoportgyökérwebhelyét.
  
2. A **Webhelyobjektumok csoportban**válassza a **Munkafolyamatok**lehetőséget. 
  
3. A **Munkafolyamatok** menüszalag **Új** szakaszában válassza az **Újrafelhasználható munkafolyamat lehetőséget.** 
  
4. Az **Újrafelhasználható munkafolyamat létrehozása** képernyőn adja meg a ** *Repair2010* **nevet. A **Platformtípus csoportban**kattintson a **SharePoint 2010-munkafolyamat**elemre, majd az **OK**gombra. 
  
1. A **Munkafolyamat** menüszalag **Mentés** szakaszában válassza a **Közzététel**lehetőséget. 
  
2. A **Munkafolyamat** menüszalag **Kezelés** szakaszában válassza a **Globális közzététel**lehetőséget. A megjelenő megerősítést kérő párbeszédpanelen válassza az **OK gombot.** 
  
3. Keresse meg a webböngészőben a webhelycsoport gyökérwebhelyét, majd érje el a **Webhelybeállítások** \> **webhelycsoport szolgáltatásait.** A Munkafolyamatok szolgáltatás **bekapcsolása:** 
  
· Ha a szolgáltatás *aktiválva* van, kattintson **az Inaktiválás gombra,** majd az **Aktiválás gombra.** 
  
· Ha a szolgáltatás *inaktiválva* van, kattintson az **Aktiválás gombra.** 
  
További információkért kérjük, olvassa el a következő [cikket](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

