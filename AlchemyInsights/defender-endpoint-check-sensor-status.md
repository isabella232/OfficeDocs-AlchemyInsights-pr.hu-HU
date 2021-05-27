---
title: Defender végpont ellenőrzése érzékelő állapota
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676178"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defender végpont ellenőrzése érzékelő állapota

Az **Érzékelővel kapcsolatos problémákat** érzékelővel kapcsolatos eszközök csempe a Biztonsági műveletek irányítópulton található. Ez a csempe információt nyújt arról, hogy az egyes eszközök képesek-e érzékelőadatok biztosítanak és kommunikáljanak a Defender for Endpoint szolgáltatással. Azt jelenti, hogy hány eszköz igényel beavatkozást, és segít azonosítani a problémás eszközöket, és lépéseket tett az ismert problémák kijavítása érdekében.

A csempén két állapotjelző jelzi, hogy hány eszköz nem jelent megfelelően a szolgáltatásnak:

- **Misconfigured** Azok az eszközök, amelyek részben jelentik az érzékelő adatait a Defender végpontnak szolgáltatásnak, és javítható konfigurációs hibákat okozhatnak.
- **Inaktív** Azok az eszközök, amelyek az elmúlt hónapban több mint hét napja nem jelentek be a Defender végpontszolgáltatásnak.

A csoportok bármelyikére kattintva az Eszközök listához irányítja a rendszer, a választási lehetőségeknek megfelelően szűrve. Az Eszközök listában az állapotlistát az alábbi állapot szerint szűrheti:

- **Aktív** Azok az eszközök, amelyek aktívan bejelentik a Defender a Végpont szolgáltatásnak.
- **Misconfigured** Azok az eszközök, amelyek részben jelentéssel látják el az érzékelő adatait a Defender végpontszolgáltatásnak, de kijavítani kell a konfigurációs hibákat. A helytelenül konfigurált eszközök az alábbi problémák egyikével vagy kombinációjával is problémákat okozhatnak:

    - Nincsenek érzékelőadatok – Az eszközök leállták az érzékelőadatok küldését. Korlátozott riasztások indíthatóak el az eszközről.
    - Károsodott kommunikáció – A készülékkel való kommunikáció károsodott. Előfordulhat, hogy nem működik a fájlok küldése mély elemzésre, fájlok blokkolása, az eszköz hálózatról való elzárása és az eszközzel való kommunikációt igénylő egyéb műveletek.
- **Inaktív** Azok az eszközök, amelyek leálltak a Végpont defender szolgáltatásnak való jelentéssel.

Az Exportálás funkcióval a teljes listát CSV formátumban letöltheti.

További információ: Az érzékelő állapotának [ellenőrzése a Microsoft Defender végponthoz szolgáltatásban.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Ha többet meg nem tudni arról, hogy mi okozta egy eszköz inaktívvá vagy helytelenül van beállítja az eszközt, tekintse meg A nem hibás érzékelőikonok kijavítva a [Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)eszközt.
