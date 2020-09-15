---
title: A meglévő monitor hibaelhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690713"
---
# <a name="troubleshoot-an-existing-monitor"></a>Meglévő monitor hibaelhárítása

Próbálkozzon ezekkel a megoldásokkal a monitor hibaelhárításához. 

**A monitor megjelenítésének frissítése:**

Nyomja le a következő billentyűket egyszerre: Windows billentyű + CTRL + SHIFT + B. Ez frissíti a grafikus illesztőprogrammal folytatott kommunikációt. A monitorok egy pillanatra villognak, és néhány másodperc elteltével visszatérhetnek.

**Monitor hardverének hibaelhárítása:**

1. Húzza ki a SZÁMÍTÓGÉPét a monitorhoz csatlakozó kábelt, és csatlakoztassa újra a monitorhoz.
2. Húzzon le minden nem alapvető eszközt a SZÁMÍTÓGÉPRŐL (például adapterek vagy dokkok).

**Ha nemrég telepített egy frissítést a SZÁMÍTÓGÉPére, visszaállíthatja a képernyő-illesztőprogramot:**

1. Válassza a **Start**gombot, írja be az **Eszközkezelőt**, és az eredményből válassza az **Eszközkezelő** lehetőséget.
2. Bontsa **ki a videokártyák** szakaszt, kattintson a jobb gombbal a videokártyához, ands válassza a **Tulajdonságok parancsot**.
3. Lépjen az **illesztőprogram** lapra, és válassza az **illesztőprogram visszaállítása**lehetőséget. <br>
Megjegyzés: Ha ez a funkció nem érhető el, vagy szürkén jelenik meg, válassza a **nem** lehetőséget az alábbi lehetőségek közül a következő lépésre való ugráshoz.
4. Előfordulhat, hogy a módosítások életbe léptetéséhez újra kell indítania a GÉPET.

**A képernyő-illesztőprogram eltávolítása és újratelepítése:**

1. Válassza a **Start**gombot, írja be az **Eszközkezelőt**, és az eredményből válassza az **Eszközkezelő** lehetőséget.
2. Bontsa **ki a videokártyák** szakaszt, kattintson a jobb gombbal a videokártyához, ands válassza az **eszköz eltávolítása**parancsot. 
3. Jelölje be az **eszközhöz tartozó illesztőprogram törlése** elem melletti jelölőnégyzetet, és válassza az **Eltávolítás**lehetőséget.<br>
Megjegyzés: Előfordulhat, hogy a rendszer kéri a számítógép újraindítását ebben a fázisban. Mielőtt újraindul, ügyeljen rá, hogy írja le a fennmaradó utasításokat.
4. Nyissa meg ismét az Eszközkezelőt.
5. Bontsa **ki a videokártyák** szakaszt, kattintson a jobb gombbal a videokártyához, és válassza az **Illesztőprogram frissítése**parancsot.
6. Válassza az **Illesztőprogram frissítése automatikus keresése** lehetőséget, és kövesse a telepítési útmutatót.