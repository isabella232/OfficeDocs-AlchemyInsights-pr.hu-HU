---
title: A beérkezett üzenetekre vonatkozó szabályok tevékenységének meghatározása a naplókban
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
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779053"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>A beérkezett üzenetekre vonatkozó szabályok tevékenységének meghatározása a naplókban

A beérkezett üzenetekre vonatkozó szabályok eseményei (a beérkezett üzenetekre vonatkozó szabályok létrehozása, módosítása és törlése) a Microsoft 365 biztonsági & megfelelőségi központban használhatók a naplózási naplóban.

1. Jelentkezzen be a [Microsoft 365 biztonsági & megfelelőségi központjába](https://protection.office.com/).

2. Nyissa meg a **keresési**  >  **napló keresési** lapját.

3. Válassza ki a dátumtartomány értékét a **kezdési dátum** és a **Záró dátum** mezőben.

4. Az **Exchange-postaláda tevékenységei**területen ellenőrizze, hogy a **tevékenységek** mező be van-e állítva: **új – a InboxRule létrehozása/módosítása/engedélyezése/letiltása a levelezési szabály letiltásával**.

5. Kattintson a **Keresés**gombra.

A találatok között válasszon egy naplózási rekordot. Kattintson a részletek menü **További információk**parancsára. A beérkezett üzenetekre vonatkozó szabály beállításairól szóló információk a **Parameters (paraméterek** ) mezőben láthatók.

További információ: [a Beérkezett üzenetek szabályát létrehozó felhasználó létrehozása](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
