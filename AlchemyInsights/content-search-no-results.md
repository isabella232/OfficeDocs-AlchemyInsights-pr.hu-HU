---
title: Nincs találat a tartalomkeresésben
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816850"
---
# <a name="no-results-from-content-searchexports"></a>Nincs találat a tartalomkeresésből/-exportálásból

A tartalomkereséssel/-exportálással kapcsolatos problémákat az adott rendszergazda által megadott megfelelőségi biztonsági szűrő miatt lehet, amely nem adja vissza az adatokat az összes rendszergazdának.

A probléma megoldásához ellenőrizze, hogy vannak-e olyan megfelelőségi biztonsági szűrők, amelyek ezt okozhatják:
1. Csatlakozás a Biztonsági és megfelelőségi központ Powershell-parancshoz
2. Futtassa az alábbi parancsmagokat:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org