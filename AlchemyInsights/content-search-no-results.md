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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058004"
---
# <a name="no-results-from-content-searchexports"></a>Nincs találat a tartalomkeresésből/-exportálásból

A tartalomkereséssel/-exportálással kapcsolatos problémákat az adott rendszergazda által megadott megfelelőségi biztonsági szűrő miatt lehet, amely nem adja vissza az adatokat az összes rendszergazdának.

A probléma megoldásához ellenőrizze, hogy vannak-e olyan megfelelőségi biztonsági szűrők, amelyek ezt okozhatják:
1. Csatlakozás Biztonsági és megfelelőségi központ Powershell-parancsa
2. Futtassa az alábbi parancsmagokat:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org