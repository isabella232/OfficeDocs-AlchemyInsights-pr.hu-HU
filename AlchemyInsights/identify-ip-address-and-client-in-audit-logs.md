---
title: IP-cím és a naplókat az ügyfél azonosítása
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909303"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-cím és a naplókat az ügyfél azonosítása

Az IP-cím, amely megfelel egy tevékenység egy felhasználó vagy rendszergazda által a naplófájlban jelenik meg. Az ügyfél adatait is naplózza. Az alábbiakban a lépéseket, hogy ilyen információk azonosítása

1. Jelentkezzen be az [Office 365 biztonsági & kompatibilitási központ](https://protection.office.com/)

2. Kattintson a **Keresés és a vizsgálat** , és válassza a **Könyvvizsgálati napló Search**.

   Ha érdekli az adott tevékenység, **tevékenységek** listából jelölje ki azt. Ha nem, minden tevékenység visszatér a kijelölt felhasználó (alapértelmezett beállítás).

   **Megjegyzés**: egyes tevékenységek nem áll rendelkezésre a **tevékenységek** menü; azonban e könyvvizsgálati elemek **Minden tevékenységek eredményének megjelenítése** a kijelölt (alapértelmezett beállítás) esetén visszatér.

3. A **felhasználók** mezőben adja meg a felhasználónevet, válassza ki a megfelelő dátumtartományt a tevékenység, és kattintson a **Keresés**.

Az eredmények a tevékenység az eredmények ablaktáblájában az IP-cím látható. Válassza ki az elemzési rekord részletes információt a **Részletek** úszó (például ügyfél, felhasználó által végzett művelet, stb.).

További tudnivalókért tanulmányozza [a feltört fiók elérésére használt számítógép IP-cím megkeresése](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
