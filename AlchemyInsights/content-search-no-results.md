---
title: Tartalom keresés eredménye
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800394"
---
# <a name="no-results-from-content-searchexports"></a>Nincs eredmény a tartalom keresési/kivitel

Problémák a tartalom keresési/kivitel nem minden adatvisszaadás bizonyos megfelelési biztonsági szűrő által adott Admin, és azt nem kommunikál a rendszergazdák minden beállítás volt lehetséges.

A probléma megoldásához ellenőrizze, hogy vannak-e bármilyen okozza-e a megfelelőség biztonsági szűrők:
1. Biztonsági és Megfelelési központba Powershell kapcsolódni
2. A következő parancsmagjaival futtatható:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org szervezet