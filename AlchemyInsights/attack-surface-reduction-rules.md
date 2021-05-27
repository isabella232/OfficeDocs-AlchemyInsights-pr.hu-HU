---
title: Támadásifelület-csökkentés szabályai
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676233"
---
# <a name="attack-surface-reduction-rules"></a>Támadásifelület-csökkentés szabályai

A fájlok vagy mappák kizárása súlyosan csökkentheti a támadásifelület-csökkentés szabályai által nyújtott védelmet. Azok a fájlok, amelyek futtatását egy szabály letiltotta volna, engedélyezettek, és nem rögzítettek jelentést vagy eseményt. Kivétel minden olyan szabályra érvényes, amely engedélyezi a kivételeket.

Az ASR-kivételek ugyanazt a szintaxist használják, mint a Microsoft Defender víruskereső kizárások. A részleteket a Kivételek beállítása és érvényesítése a Microsoft Defender víruskereső [olvassa el.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) A problémák elkerülése érdekében tekintse át a Kivételek definiálása során gyakran használt hibákat ismertető [ismertetőt.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Nem minden asr-szabály támogatja a kivételeket. Ha ellenőrizni tudja, hogy a szabály támogatja-e a kivételeket, tekintse meg a Támadásifelület-csökkentés szabályai [táblázatot.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Támadásifelület-csökkentés szabályai

A szervezet támadási felülete magában foglalja az összes olyan helyet, ahol a támadóknak feltörhetik a szervezet eszközeit vagy hálózatait. A támadási felület csökkentése azt jelenti, hogy védelmet nyújt a szervezet eszközeinek és hálózatának, így a támadóknak kevesebb módszer áll a támadásra. A támadásifelület-csökkentés szabályainak konfigurálása segíthet a Microsoft Defender végponthoz való beállításában.

További információ:

- [ASR-szabály GUID-ként való leképezésének elnevezése](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- AsR rules requirements:
    - [Windows 10 Pro 1709-es vagy újabb verzió](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise 1709-es vagy újabb verzió](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, version 1803 (Semi-Annual Channel) or later](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>A helyes kivétel azonosítása

1. Keresse meg a 1121-es vagy 1122-es eseményazonosítót a Microsoft-Windows-Windows Defender/Műveleti naplóban.

1. Mérje fel a blokk esetét és környezetét, és győződjön meg arról, hogy ebben az esetben fel kell oldani a blokkolást.

1. Olvassa el a Path (Útvonal) értéket az esemény részleteiben, amely a kivételt meghatározó érték.
    - A kivételt a lehető legszigorúbbra kell tenni.
    - Szükség esetén alkalmaz egy helyettesítő karaktereket (például Felhasználói változó cseréje).

1. A kivétel alkalmazása a telepítési igényeknek megfelelően. Részletes információkért lásd: [Támadásifelület-csökkentés szabályainak testreszabása.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Kivételt nem ad vissza

1. Állapítsa meg, hogy a szabály támogatja-e a kivételeket. További információ: [Támadásifelület-csökkentés szabályai.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Tekintse át az alkalmazott kivételeket, és ellenőrizze az elkallott vagy tévesen értelmezett helyettesítő karaktereket az esemény adataival. További információ: Támogatott [kivételtípusok](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. ha a szabály túl nagy hatása van, érdemes megfontolni a szabály (vissza) naplózási módba való áthelyezését további ellenőrzéshez. Részletes információkért lásd: [A Microsoft Defender a végpontok funkcióinak naplózási üzemmódban való használata.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Támogatási adatok összegyűjtése támogatási eset megnyitásához a következő paranccsal:
    
   ** MDEClientAnalyzer.cmd -v**

    További információért lásd: A számítógépeknek a [Microsoft Defender végpontokkal](issues-with-onboarding-machines.md)kapcsolatos problémái.
