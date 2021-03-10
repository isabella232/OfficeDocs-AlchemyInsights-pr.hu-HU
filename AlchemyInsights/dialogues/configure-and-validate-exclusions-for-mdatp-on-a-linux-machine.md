---
title: Kizárások konfigurálása és ellenőrzése az MDATP-hez Linux-gépen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694265"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>Kizárások konfigurálása és ellenőrzése az MDATP-hez Linux-gépen

Az MDATP-vizsgálatból kizárhat bizonyos fájlokat, mappákat, folyamatokat és folyamat által megnyitott fájlokat. A kizárások segítenek megelőzni a szoftverek és fájlok egyedi vagy testre szabott észlelését. A kizárások az MDATP által okozott teljesítményproblémák csökkentésében is segítenek.

További információt a Kivételek konfigurálása és érvényesítése a [Linux MDATP-hez.](https://go.microsoft.com/fwlink/?linkid=2144517)

> [!IMPORTANT]
> A cikkben ismertetett kizárások nem vonatkoznak a Linux MDATP egyéb funkcióira, beleértve a végpontok észlelését és a válasz (EDR) funkcióit. A cikkben ismertetett módszerekkel kizárt fájlok továbbra is elindíthatják az EDR-riasztásokat és más észlelési funkciókat.
