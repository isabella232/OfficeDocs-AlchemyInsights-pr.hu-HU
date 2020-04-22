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
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716390"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Ip-cím és ügyfél azonosítása a naplókban

A Microsoft 365-felhasználó vagy -rendszergazda tevékenységének megfelelő IP-cím a naplókban jelenik meg. Az ügyféladatok is naplózva lesznek. Az alábbi lépésekkel azonosíthatók az ilyen információk

1. Jelentkezzen be a [Microsoft 365 Biztonsági & megfelelőségi központjába.](https://protection.office.com/)

2. Nyissa meg a **Keresési** > **napló keresési naplójának keresési** lapját.

   Ha érdekel egy adott tevékenység, válassza ki a **Tevékenységek** listából. Ha nem, akkor a kijelölt felhasználó minden tevékenysége visszakerül (alapértelmezett beállítás).

   **Megjegyzés**: Előfordulhat, hogy bizonyos tevékenységek nem érhetők el a **Tevékenységek** menüben; ezek a naplózási elemek azonban akkor kerülnek visszaadásra, ha **az összes tevékenység eredményének megjelenítése** be van jelölve (alapértelmezett beállítás).

3. Adja meg a felhasználónevet a **Felhasználók** mezőben, válassza ki a tevékenységhez megfelelő dátumtartományt, majd kattintson a **Keresés gombra.**

Az eredményekben az adott tevékenység IP-címét láthatja az eredmények ablaktáblában. Válassza ki a naplózási rekordot a **Részletek** úszó panelrészletes információinak megtekintéséhez (például Ügyfél, Műveletet végző felhasználó stb.).

További információt [a feltört fiók eléréséhez használt számítógép IP-címének megkeresése](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)című témakörben talál.
