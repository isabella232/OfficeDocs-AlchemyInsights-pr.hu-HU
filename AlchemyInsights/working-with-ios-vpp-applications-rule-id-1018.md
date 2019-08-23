---
title: IOS VPP alkalmazások szabály azonosító 1018 használata
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558000"
---
# <a name="working-with-ios-vpp-applications"></a>IOS VPP-alkalmazások használata

Olvassa el a további információt a szolgáltatások, megkötések és lépései [vásárolt Microsoft Intune-vásárlás program iOS alkalmazások kezelése](https://docs.microsoft.com/intune/vpp-apps-ios) az Apple kötet beszerzési Program és a támogatást, akkor a Microsoft Intune használatát.
  
 **Gyakori kérdések:** "A felhasználók számára kiosztott az iOS VPP app, de a telepítés sikertelen volt."
  
- Ez akkor fordulhat elő, egyetlen VPP token használata esetén több mobileszközön management szolgáltató között. VPP tokenek az Apple csak egy szolgáltató használhatók. Több szolgáltató használt VPP tokent, ha a jogkivonat Intune újra kell feltölteni.

- A telepítés is sikertelen lehet, ha létesítmények teljes száma meghaladja a licencek számát. Használati jelentés a licencek megtekintéséhez nyissa meg az **apps Intune Mobile** \> **App licencek** lapon. Visszanyeréséhez használt licencek, lásd: [cikkben.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
