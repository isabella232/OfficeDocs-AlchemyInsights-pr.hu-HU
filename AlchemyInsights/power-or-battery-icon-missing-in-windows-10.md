---
title: Hiányzik a főkapcsoló- vagy akkumulátor ikon a Windows 10 rendszerben
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 82d41844de1eafdf7e0cc38f91416f3b71868e3d5d1b3eb8be0f10abd701ddc8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973323"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Hiányzik a főkapcsoló- vagy akkumulátor ikon a Windows 10 rendszerben

Ha Windows 10-es eszköze rendelkezik akkumulátorral (például szünetmentes táphoz USB-n keresztül csatlakoztatott laptop, táblagép vagy asztali számítógép), általában a tálcán az óra mellett látható egy áram- vagy akkumulátor ikon, például:

![Akkumulátor ikon](media/battery-icon.png)

Ha nem látja ezt az ikont, lehet, hogy el van rejtve:

1. Ugorjon a **[Gépház > Személyre szabás > Tálca](ms-settings:taskbar?activationSource=GetHelp)** lapra.

2. Az Értesítési területen kattintson **A tálcán megjelenő ikonok kiválasztása** lehetőségre.

3. Ezután keresse meg **Főkapcsoló** elemet a listában, és a kapcsolót állítsa a **Be** értékre.

    ![A főkapcsoló ikon megjelenítése a tálcán](media/power-icon-on.png)

**Hibaelhárítás**

Ha követte a fenti utasításokat, és a **Főkapcsoló** váltója kiszürkül vagy nem látható, írja be a tálca keresőmezőjébe az **eszközkezelő** kifejezést, majd a találatok listájában válassza az **Eszközkezelő** elemet. Az **Akkumulátorok** csoportban kattintson jobb gombbal az eszköz akkumulátorára, kattintson a **Letiltás** elemre, majd kattintson az **Igen** lehetőségre. Várjon néhány másodpercet, majd kattintson jobb gombbal az akkumulátorra, és válassza az **Engedélyezés** lehetőséget. Ezután indítsa újra az eszközt.

Ha követte fenti utasításokat, de az akkumulátor ikonja nem jelenik meg a tálcán, írja be tálcán a keresőmezőbe a **feladatkezelő** kifejezést, majd a találatok listájában válassza a **Feladatkezelő** elemet. A **Név** csoportban található **Folyamatok** lapon kattintson jobb gombbal az **Intéző** elemre, majd kattintson az **Újraindítás** parancsra.
