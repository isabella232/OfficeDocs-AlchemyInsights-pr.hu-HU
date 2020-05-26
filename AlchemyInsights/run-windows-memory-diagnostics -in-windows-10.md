---
title: A Windows memóriadiagnosztika futtatása a Windows 10-ben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357791"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>A Windows memóriadiagnosztika futtatása a Windows 10-ben

Ha a Windows és a számítógépen lévő alkalmazások összeomlanak, lefagynak vagy instabil módon működnek, akkor lehet, hogy probléma van a számítógép memóriájával (RAM). A Windows memóriadiagnosztika futtatásával ellenőrizheti, hogy vannak-e problémák a számítógép RAM memóriájával kapcsolatban.

A tálca keresőmezőjébe írja be a **memóriadiagnosztika parancsot,** majd válassza a **Windows memóriadiagnosztika**lehetőséget. 

A diagnosztika futtatásához a számítógépnek újra kell indulnia. Lehetősége van arra, hogy azonnal újrainduljon (mentse el a munkáját, és először zárja be a megnyitott dokumentumokat és e-maileket), vagy ütemezze a diagnosztikát úgy, hogy automatikusan fusson a számítógép következő újraindításakor:

![Windows memóriadiagnosztika](media/windows-memory-diagnostic.png)

Amikor a számítógép újraindul, a **Windows memóriadiagnosztikai eszköz** automatikusan elindul. Az állapot és a folyamat a diagnosztika futása közben jelenik meg, és lehetősége van a diagnosztika megszakítására az **ESC** billentyű nek a billentyűzeten való megnyomásával.

Amikor a diagnosztika befejeződött, a Windows a szokásos módon indul el.
Közvetlenül az újraindítás után, amikor az asztal megjelenik, egy értesítés jelenik meg (a **műveletközpont** ikonja mellett a tálcán), jelezve, hogy találtak-e memóriahibákat. Például:

A Műveletközpont ikonja: ![A Műveletközpont ikonja](media/action-center-icon.png) 

És egy minta értesítés: ![Nincsmemória-hiba](media/no-memory-errors.png)

Ha nem fogadott el az értesítést, a **műveletközpont** ikonja a tálcán a **Műveletközpont** megjelenítéséhez és az értesítések görgethető listájának megjelenítéséhez.

A részletes információk áttekintéséhez írja be az **eseményt** a tálca keresőmezőjébe, és válassza az **Eseménynapló**lehetőséget. Az **Eseménynapló**bal oldali ablaktáblájában keresse meg a **Windows naplók > System ablakot.** A jobb oldali ablaktáblában olvassa be a listát, miközben a **Forrás** oszlopot nézi, amíg meg nem jelennek a **MemoryDiagnostics-Results**forrásértékű események. Jelölje ki az egyes eseményeket, és tekintse meg az eredményadatokat a lista alatti **Általános** lap alatt található mezőben.
