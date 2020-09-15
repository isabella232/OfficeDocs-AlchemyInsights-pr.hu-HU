---
title: A hiányzó munkafolyamat aktiválása sikertelen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667088"
---
# <a name="missing-workflow-failed-to-activate"></a>A hiányzó munkafolyamat aktiválása sikertelen

A Microsoft SharePoint-webhelycsoportban nem lehet globálisan újrafelhasználható munkafolyamatot (például "jóváhagyás – SharePoint 2010") hozzáadni egy listához vagy tárhoz.
  
A probléma megoldásához kövesse az alábbi lépéseket: 
  
1. Nyissa meg a webhelycsoport legfelső szintű webhelyét a SharePoint Designer 2013-ban.
  
2. A **hely objektumai**csoportban válassza a **munkafolyamatok**elemet. 
  
3. A **munkafolyamatok** menüszalagjának **új** szakaszában válassza az **újból felhasználható munkafolyamat**lehetőséget. 
  
4. Az **újrafelhasználható munkafolyamat létrehozása** űrlapon írja be a * * *Repair2010* * * nevet. **Platform típusa**esetén kattintson a **SharePoint 2010 munkafolyamat**elemre, majd kattintson **az OK**gombra. 
  
1. A **munkafolyamat** menüszalagjának **Mentés** szakaszában válassza a **Közzététel**lehetőséget. 
  
2. A **munkafolyamat** menüszalagjának **Manage (kezelés** ) szakaszában válassza a **globális közzététel**lehetőséget. A megjelenő megerősítést kérő párbeszédpanelen válassza az **OK gombot**. 
  
3. A webböngészőben keresse meg a webhelycsoport legfelső szintű webhelyét, és nyissa meg a webhely **beállításai** – webhelycsoport \> **funkcióit**. Ezután kapcsolja be a **munkafolyamatok** funkcióját: 
  
· Ha a funkció  *aktiválva*  van, kattintson az **Inaktiválás gombra,** majd az **aktiválás**parancsra. 
  
· Ha a funkció  *inaktiválva*  van, kattintson az **aktiválás**gombra. 
  
További információért olvassa el a következő [cikket](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

