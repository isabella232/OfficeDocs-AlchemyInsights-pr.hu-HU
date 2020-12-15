---
title: A tartalom keresése/exportálása során a találatok között nincs eredmény
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678678"
---
# <a name="no-results-returned-during-content-searchexport"></a>A tartalom keresése/exportálása során a találatok között nincs eredmény

Ha problémák lépnek fel a következő eDiscovery-esetekben:

- A tartalom keresése/exportálása adatvesztést vagy nem várt adatot ad eredményül.
- a eDiscovery keresés vagy exportálás nem sikerült

Ennek oka az lehet, hogy egy adott rendszergazda által beállított bizonyos megfelelőségi biztonsági szűrők miatt nem lettek közölve az összes rendszergazda.

A probléma megoldásához győződjön meg arról, hogy vannak-e olyan megfelelőségi biztonsági szűrők, amelyek a következő problémákat okozhatják:

1. Csatlakozás a biztonsági és megfelelőségi központ Powershellhez
2. Futtassa az alábbi parancsmaggal található:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

A megfelelőségi biztonsági szűrőkről további információt a [tartalom keresése engedélyek szűrése](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search) című témakörben talál.
