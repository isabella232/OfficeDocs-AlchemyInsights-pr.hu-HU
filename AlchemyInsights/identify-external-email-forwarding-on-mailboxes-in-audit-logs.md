---
title: Külső e-mail továbbítás a naplókat a postafiókok azonosítása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383099"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ha külső e-mail továbbító van beállítva a postafiókok azonosítása

Ha a felhasználó külső e-mail továbbítási postafiók azt állítja be, a tevékenység részeként a **Set-Mailbox** parancsmag naplózza a rendszer. A könyvvizsgálati napló keresés használata a biztonsági & Megfelelési központba tevékenység tekintheti meg.

1. Jelentkezzen be az [Office 365 biztonsági & kompatibilitási központ](https://protection.office.com/)

2. Kattintson a **Keresés és a vizsgálat** , és válassza a **Könyvvizsgálati napló Search**.

3. Jelöljük ki a dátumot a **Kezdő dátum** és **Záró dátum** mezőket. Nem kell adnia a felhasználónevet. Ellenőrizze, hogy a **tevékenységeket** a mező értéke **Minden tevékenység eredmény megjelenítése**.

4. Kattintson a **Keresés**gombra.

Az eredmények között kattintson a **Szűrés eredménye** , és a tevékenység szűrő mezőbe írja be **Set-Mailbox** . Válassza ki az eredmények tételt generál. Kattintson a **Részletek** úszó **További információt**. Akkor állapítható meg, ha a tevékenységhez kapcsolódó e-mail továbbító minden naplóbejegyzés részleteit megtekinteni.

- **ObjectId**: az alias érték a postafiók módosításának.

- **Paraméterek**: _ForwardingSmtpAddress_ jelzi, hogy a cél e-mail címet.

- **UserId**: A felhasználó e-mail továbbítási konfigurálva az **objektumazonosító** mezőben a postafiók.

További információért lásd: [aki postaládához továbbítása e-mail beállítás meghatározása](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
