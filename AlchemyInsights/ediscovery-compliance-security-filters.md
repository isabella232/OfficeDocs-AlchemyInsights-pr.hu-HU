---
title: Nincs találat a tartalomkeresés/-exportálás során
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101268"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nincs találat a tartalomkeresés/-exportálás során

Ha problémákat tapasztal az alábbi elektronikus észlelési forgatókönyvekkel kapcsolatban:

- A tartalomkeresés/-exportálás nem ad vissza adatokat vagy váratlan adatokat.
- Sikertelen keresés vagy exportálás az elektronikus adatfelkeresésben

Ezt okozhatja bizonyos megfelelőségi biztonsági szűrők, amelyek beállítása egy adott rendszergazda által történt, és nem lett közölve az összes rendszergazdával.

A probléma megoldásához ellenőrizze, hogy vannak-e olyan megfelelőségi biztonsági szűrők, amelyek ezeket a problémákat okozhatják:

1. Csatlakozás Biztonsági és megfelelőségi központ Powershell-parancsa
2. Futtassa az alábbi parancsmagokat:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

A megfelelőségi biztonsági szűrőkről további információt az Engedélyszűrés [a tartalomkereséshez](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
