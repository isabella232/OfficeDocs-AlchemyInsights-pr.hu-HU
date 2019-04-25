---
title: Külső e-mail továbbítás a naplókat a postafiókok azonosítása
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417214"
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
