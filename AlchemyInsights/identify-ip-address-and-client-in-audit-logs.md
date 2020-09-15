---
title: Az IP-cím és az ügyfél meghatározása a naplókban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668312"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Az IP-cím és az ügyfél meghatározása a naplókban

A Microsoft 365-felhasználók vagy-rendszergazdák által egy tevékenységhez tartozó IP-cím megjelenik a naplókban. Az ügyfél adatai is naplózásra kerülnek. Az alábbi lépésekkel azonosíthatja ezeket az információkat

1. Jelentkezzen be a [Microsoft 365 biztonsági & megfelelőségi központjába](https://protection.office.com/).

2. Nyissa meg a **keresési**  >  **napló keresési** lapját.

   Ha egy adott tevékenység érdekli, jelölje ki a **tevékenységek** listából. Ha nem, a program az összes tevékenységet visszaadja a kijelölt felhasználónak (alapértelmezett beállítás).

   **Megjegyzés**: Előfordulhat, hogy bizonyos tevékenységek nem érhetők el a **tevékenységek** menüben; Ha azonban az **összes tevékenység eredményének megjelenítése** jelölőnégyzet be van jelölve, akkor a rendszer ezeket a naplózási elemeket adja vissza (alapértelmezett beállítás).

3. Adja meg a felhasználónevet a **felhasználók** mezőben, válassza ki a tevékenységhez megfelelő dátumtartományt, majd kattintson a **Keresés**gombra.

A találatok között láthatja az adott tevékenységhez tartozó IP-címet az eredmények munkaablakban. Válassza a könyvvizsgálati rekordot, ha részletes információkat szeretne látni a részletek (például ügyfél, felhasználó, művelet stb.) **részleteiről** .

További információért olvassa el a [sérült fiók eléréséhez használt számítógép IP-címének megkeresése](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)című témakört.
