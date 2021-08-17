---
title: IP-cím és ügyfél azonosítása a naplókban
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
ms.openlocfilehash: 080b3df3934781ebf0d0cd5243787bf6975fc5f123b5b1593c0b6d9ada4eae5d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887502"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-cím és ügyfél azonosítása a naplókban

Az IP-cím, amely egy felhasználó vagy rendszergazda Microsoft 365 tevékenységének felel meg, megjelenik a naplókban. A program az ügyféladatokat is naplózza. Az ilyen információk azonosításának lépései

1. Jelentkezzen be a [Microsoft 365 megfelelőségi központba.](https://protection.office.com/)

2. Lépjen a Keresési  >  **napló keresési lapjára.**

   Ha egy adott tevékenységre kíváncsi, válassza ki azt a Tevékenységek **listából.** Ha nem, a rendszer a kijelölt felhasználó összes tevékenységét visszaadja (alapértelmezett beállítás).

   **Megjegyzés:** Előfordulhat, hogy egyes tevékenységek nem érhetők el a **Tevékenységek menüben;** ezeket a naplóelemeket azonban a program akkor is visszaadja, ha az Eredmény megjelenítése **az összes** tevékenységhez beállítás van megjelölve (alapértelmezett beállítás).

3. Adja meg a felhasználónevet a Felhasználók **mezőben,** válassza ki a tevékenységhez a megfelelő dátumtartományt, majd kattintson a Keresés **gombra.**

A találatok között láthatja a tevékenység IP-címét az eredménypanelen. A naplórekord kiválasztásával részletes  információkat láthat a Részletek előjelben (például Ügyfél, A műveletet végrehajtotta stb.).

További információ: Az feltört fiókok eléréséhez használt számítógép [IP-címének megkeresása.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
