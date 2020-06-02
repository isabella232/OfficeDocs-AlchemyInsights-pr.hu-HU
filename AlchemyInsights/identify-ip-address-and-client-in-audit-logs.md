---
title: Ip-cím és ügyfél azonosítása a naplókban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508918"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Ip-cím és ügyfél azonosítása a naplókban

A Microsoft 365-felhasználó vagy -rendszergazda tevékenységének megfelelő IP-cím a naplókban jelenik meg. Az ügyféladatok is naplózva lesznek. Az alábbi lépésekkel azonosíthatók az ilyen információk

1. Jelentkezzen be a [Microsoft 365 Biztonsági & megfelelőségi központjába.](https://protection.office.com/)

2. Nyissa meg a **Keresési**  >  **napló keresési naplójának keresési** lapját.

   Ha érdekel egy adott tevékenység, válassza ki a **Tevékenységek** listából. Ha nem, akkor a kijelölt felhasználó minden tevékenysége visszakerül (alapértelmezett beállítás).

   **Megjegyzés**: Előfordulhat, hogy bizonyos tevékenységek nem érhetők el a **Tevékenységek** menüben; ezek a naplózási elemek azonban akkor kerülnek visszaadásra, ha **az összes tevékenység eredményének megjelenítése** be van jelölve (alapértelmezett beállítás).

3. Adja meg a felhasználónevet a **Felhasználók** mezőben, válassza ki a tevékenységhez megfelelő dátumtartományt, majd kattintson a **Keresés gombra.**

Az eredményekben az adott tevékenység IP-címét láthatja az eredmények ablaktáblában. Válassza ki a naplózási rekordot a **Részletek** úszó panelrészletes információinak megtekintéséhez (például Ügyfél, Műveletet végző felhasználó stb.).

További információt [a feltört fiók eléréséhez használt számítógép IP-címének megkeresése](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)című témakörben talál.
