---
title: A beérkezett üzenetek szabályával kapcsolatos tevékenységek azonosítása a naplókban
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891297"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>A beérkezett üzenetek szabályával kapcsolatos tevékenységek azonosítása a naplókban

A naplókereséssel megtekintheti a beérkezett Microsoft 365 Megfelelőségi központ eseményeket (a beérkezett üzenetekre vonatkozó szabályok létrehozását, módosítását és törlését).

1. Tegye a következők valamelyikét:
   - A Microsoft 365 Megfelelőségi központ a <https://compliance.microsoft.com> Megoldásvizsgálat  \> **hoz.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://compliance.microsoft.com/auditlogsearch> használja: .
   - A (Microsoft 365 Defender) portálon a <https://security.microsoft.com> Audit **(Naplózás) stb.** Vagy ha közvetlenül a Naplózás **lapra,** a következőt <https://security.microsoft.com/auditlogsearch> használja: .

2. A Naplózás **lap** Keresés **lapján** adja meg az alábbi beállításokat:
   - **Dátum- és időtartomány:** Válassza ki a dátum-/időtartományt a **Kezdő** és a **Záró** mezőben.
   - **Tevékenységek:** Válasszon egyet vagy többet az alábbi értékek közül:
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App.**
     - **Beérkezett üzenetekre vonatkozó szabályok frissítése Outlook ügyfélprogramból**

3. Ha végzett, kattintson a Keresés **gombra.** A tevékenységek az új Naplókeresés **lapon jelennek** meg.

4. Jelöljön ki egy tevékenységet az eredmények között a részleteket tartalmazó úszó panel megnyitásához. A beérkezett üzenetekre vonatkozó szabályok beállításairól a Parameters mezőben tájékoztató információk **jelennek** meg.

További információ: Annak megállapítása, hogy egy felhasználó hozott-e létre beérkezett [üzenetekre vonatkozó szabályt.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
