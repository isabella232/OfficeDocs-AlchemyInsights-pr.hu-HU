---
title: A hiányzó munkafolyamat nem aktiválható
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065430"
---
# <a name="missing-workflow-failed-to-activate"></a>A hiányzó munkafolyamat nem aktiválható

A Microsoft SharePoint-webhelycsoportokban nem lehet globálisan újrahasználható munkafolyamatot (például "Jóváhagyás – SharePoint 2010") hozzáadni egy listához vagy tárhoz.
  
A probléma megoldásához kövesse az alábbi lépéseket: 
  
1. Nyissa meg a webhelycsoport gyökérwebhelyét a SharePoint Designer 2013-ban.
  
2. A **Webhelyobjektumok alatt** válassza **a Munkafolyamatok lehetőséget.** 
  
3. A **Munkafolyamatok menüszalag** Új szakaszában **válassza** az **Újrahasználható munkafolyamat lehetőséget.** 
  
4. Az **Újrahasználható** munkafolyamat létrehozása űrlapon adja meg a ** *Javítás2010* ** nevet. A **Platformtípus gombra** kattintva SharePoint **2010-munkafolyamat gombra,** majd kattintson az **OK gombra.** 
  
1. A Munkafolyamat **menüszalagJának** Mentés szakaszában **válassza** a Közzététel **elemet.** 
  
2. A Munkafolyamat **menüszalag** kezelés szakaszában **válassza** a Közzététel **globálisan lehetőséget.** A megjelenő megerősítést kérő párbeszédpanelen válassza az **OK gombot.** 
  
3. Egy webböngészőben keresse meg a webhelycsoport gyökérwebhelyét, és keresse meg a Webhelycsoport **Gépház** \> **webhelycsoport-funkciókat.** Ezután kapcsolót a **Munkafolyamatok funkcióhoz:** 
  
· Ha a funkció *aktiválva* van, kattintson az Inaktiválás, **majd** az Aktiválás **elemre.** 
  
· Ha a funkció inaktiválva *van,* kattintson az Aktiválás **gombra.** 
  
További információt a következő cikkben [talál:](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

