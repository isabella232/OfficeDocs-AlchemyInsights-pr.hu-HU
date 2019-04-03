---
title: Az Office 365 speciális veszély védelmi (ATP) kapcsolatos problémák elhárítása
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030992"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Office 365 ATP problémáinak elhárítása

- **Az e-mail üzenet kézbesítési értesítés késedelem**? Próbálja meg használni a dinamikus kiszállítás beállítást az ATP biztonságos mellékletek házirendek. E-mail üzenet kézbesítési késések így elkerülhető, miközben védi a címzettek a rosszindulatú fájlokat.
- A **kívánt jelentés hamis pozitív vagy hamis negatív**? E hivatkozás segítségével a fájl elemzéséhez nyújt:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Tudja, hogy engedélyezze a biztonságos kapcsolatok ATP védelmet a szervezet tagjai között küldött e-mail**? Kövesse az alábbi lépéseket:
    1. Ugrás a https://protection.office.com, és jelentkezzen be.
    2. Ugrás a **fenyegetés kezelése** > **politika** > **Biztonságos kapcsolatokat**.
    3. **A megadott címzetteknek érvényes házirendek**szerkesztése vagy hozzáadása egy házirend.
    4. Válassza ki **a szervezeten belül elküldött üzenetek biztonságos hivatkozásokat alkalmaz**.
    5. A házirend mentése, és lehetővé teszi a módosítások a datacenter keresztül haladva körülbelül 30 percig.
- További segítség az Ígérethez rendelkezésre álló mennyiség, olvassa el az [Office 365 speciális veszély védelmi](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).