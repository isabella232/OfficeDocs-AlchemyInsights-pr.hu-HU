---
title: A hiányzó munkafolyamat ot nem sikerült aktiválni
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762103"
---
# <a name="missing-workflow-failed-to-activate"></a>A hiányzó munkafolyamat ot nem sikerült aktiválni

Microsoft SharePoint-webhelycsoportban nem adhat hozzá globálisan újrafelhasználható munkafolyamatot (például "Jóváhagyás – SharePoint 2010") listához vagy tárhoz.
  
A probléma megoldásához hajtsa végre az alábbi lépéseket: 
  
1. Nyissa meg a SharePoint Designer 2013 webhelycsoportgyökérwebhelyét.
  
2. A **Webhelyobjektumok csoportban**válassza a **Munkafolyamatok**lehetőséget. 
  
3. A **Munkafolyamatok** menüszalag **Új** szakaszában válassza az **Újrafelhasználható munkafolyamat lehetőséget.** 
  
4. Az **Újrafelhasználható munkafolyamat létrehozása** képernyőn adja meg a ** *Repair2010* **nevet. A **Platformtípus csoportban**kattintson a **SharePoint 2010-munkafolyamat**elemre, majd az **OK**gombra. 
  
1. A **Munkafolyamat** menüszalag **Mentés** szakaszában válassza a **Közzététel**lehetőséget. 
  
2. A **Munkafolyamat** menüszalag **Kezelés** szakaszában válassza a **Globális közzététel**lehetőséget. A megjelenő megerősítést kérő párbeszédpanelen válassza az **OK gombot.** 
  
3. Keresse meg a webböngészőben a webhelycsoport gyökérwebhelyét, majd érje el a **Webhelybeállítások** \> **webhelycsoport szolgáltatásait.** Ezután kapcsolja be a **Munkafolyamatok** funkciót: 
  
· Ha a szolgáltatás *aktiválva* van, kattintson **az Inaktiválás gombra,** majd az **Aktiválás gombra.** 
  
· Ha a szolgáltatás *inaktiválva* van, kattintson az **Aktiválás gombra.** 
  
További információkért kérjük, olvassa el a következő [cikket](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

