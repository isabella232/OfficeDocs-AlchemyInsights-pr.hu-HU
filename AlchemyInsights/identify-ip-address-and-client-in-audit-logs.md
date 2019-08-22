---
title: IP-cím és a naplókat az ügyfél azonosítása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539031"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>IP-cím és a naplókat az ügyfél azonosítása

Az IP-cím, amely megfelel az Office 365-felhasználó vagy rendszergazda által tevékenység jelenik meg a naplókat. Az ügyfél adatait is naplózza. Az alábbiakban a lépéseket, hogy ilyen információk azonosítása

1. Jelentkezzen be az [Office 365 biztonsági & Megfelelési központba](https://protection.office.com/).

2. Keresse fel a **keresési** > **Audit napló** keresőlap.

   Ha érdekli az adott tevékenység, **tevékenységek** listából jelölje ki azt. Ha nem, minden tevékenység visszatér a kijelölt felhasználó (alapértelmezett beállítás).

   **Megjegyzés**: egyes tevékenységek nem áll rendelkezésre a **tevékenységek** menü; azonban e könyvvizsgálati elemek **Minden tevékenységek eredményének megjelenítése** a kijelölt (alapértelmezett beállítás) esetén visszatér.

3. A **felhasználók** mezőben adja meg a felhasználónevet, válassza ki a megfelelő dátumtartományt a tevékenység, és kattintson a **Keresés**.

Az eredmények a tevékenység az eredmények ablaktáblájában az IP-cím látható. Válassza ki az elemzési rekord részletes információt a **Részletek** úszó (például ügyfél, felhasználó által végzett művelet, stb.).

További tudnivalókért tanulmányozza [a feltört fiók elérésére használt számítógép IP-cím megkeresése](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
