---
title: Nem lehet 2010-es jóváhagyási munkafolyamatot hozzáadni
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: e74c842f8b4be321664f8c2f1f58c570d0724d80edb1264add0647bf313bc82f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020338"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Nem lehet 2010-es jóváhagyási munkafolyamatot hozzáadni

A Microsoft SharePoint-webhelycsoportokban nem lehet globálisan újrahasználható munkafolyamatot (például "Jóváhagyás – SharePoint 2010") hozzáadni egy listához vagy tárhoz.
  
A probléma megoldásához kövesse az alábbi lépéseket: 
  
1. Nyissa meg a webhelycsoport gyökérwebhelyét a SharePoint Designer 2013-ban.
  
2. A **Webhelyobjektumok alatt** válassza **a Munkafolyamatok lehetőséget.** 
  
3. A **Munkafolyamatok menüszalag** Új szakaszában **válassza** az **Újrahasználható munkafolyamat lehetőséget.** 
  
4. Az **Újrahasználható** munkafolyamat létrehozása űrlapon adja meg a ** *Javítás2010* ** nevet. A **Platformtípus gombra** kattintva SharePoint **2010-munkafolyamat gombra,** majd kattintson az **OK gombra.** 
  
1. A Munkafolyamat **menüszalagJának** Mentés szakaszában **válassza** a Közzététel **elemet.** 
  
2. A Munkafolyamat **menüszalag** kezelés szakaszában **válassza** a Közzététel **globálisan lehetőséget.** A megjelenő megerősítést kérő párbeszédpanelen válassza az **OK gombot.** 
  
3. Egy webböngészőben keresse meg a webhelycsoport gyökérwebhelyét, és keresse meg a Webhelycsoport **Gépház** \> **webhelycsoport-funkciókat.** A Munkafolyamatok **funkció be-/ki- és bekapcsolása:** 
  
· Ha a funkció *aktiválva* van, kattintson az Inaktiválás, **majd** az Aktiválás **elemre.** 
  
· Ha a funkció inaktiválva *van,* kattintson az Aktiválás **gombra.** 
  
További információt a következő cikkben [talál:](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

