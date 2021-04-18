---
title: A Windows memóriadiagnosztika futtatása a Windows 10-ben
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826669"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>A Windows memóriadiagnosztika futtatása a Windows 10-ben

Ha a Windows és a PC-n telepített alkalmazások összeomlanak, lefagynak vagy instabilan működnek, probléma lehet a PC memóriájával (a RAM-mal). A Windows memóriadiagnosztika futtatásával ellenőrizheti, hogy vannak-e problémák a PC RAM-jával kapcsolatban.

A tálcán lévő keresőmezőbe írja be a **memóriadiagnosztika** szót, majd válassza ki a **Windows memóriadiagnosztika** alkalmazást. 

A diagnosztika futtatásához a PC-nek újra kell indulnia. Lehetősége van azonnal újraindítani a PC-t (először mentse a munkáját, és zárja be a megnyitott dokumentumokat és e-maileket), vagy beütemezheti a diagnosztika automatikus futtatását a PC következő újraindulásakor:

![Windows memóriadiagnosztika](media/windows-memory-diagnostic.png)

A PC újraindítása után automatikusan futni kezd a **Windows memóriadiagnosztika eszköz**. A diagnosztika futása során megjelenik az állapot és a folyamat előrehaladása, és a billentyűzeten levő **ESC** billentyű lenyomásával megszakíthatja a diagnosztikát.

A diagnosztika befejeződése után a Windows a szokásos módon elindul.
Közvetlenül az újraindítás után, az asztal megjelenésekor megjelenik egy értesítés (a tálcán lévő **Műveletközpont** ikon mellett), amely jelzi, hogy találhatók-e memóriahibák. Például:

Ez itt a Műveletközpont ikonja: ![Műveletközpont ikon](media/action-center-icon.png) 

Ez pedig egy példa az értesítésre: ![Nincs memóriahiba](media/no-memory-errors.png)

Ha elmulasztotta az értesítést, a tálcán lévő **Műveletközpont** ikon kiválasztásával megjelenítheti a **Műveletközpontot**, amely tartalmazza az értesítések görgethető listáját.

A részletes információk áttekintéséhez írja be az **esemény** szót a tálcán található keresőmezőbe, majd válassza az **Eseménynapló** alkalmazást. Az **Eseménynapló** bal oldali ablaktáblájában lépjen a **Windows-naplók > Rendszer** elemre. A jobb oldali ablaktáblában fentről lefelé haladva nézze át a listát, és figyelje a **Forrás** oszlopot, amíg nem talál olyan eseményeket, amelyeknél a Forrás értéke **MemoryDiagnostics-Results**. Jelölje ki sorban mindegyik ilyen eseményt, és a lista alatti **Általános** lapon levő mezőben tekintse meg az eredményeket.
