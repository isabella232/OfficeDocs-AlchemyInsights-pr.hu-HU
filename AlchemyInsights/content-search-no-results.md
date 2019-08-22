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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516781"
---
# <a name="no-results-from-content-searchexports"></a>Nincs eredmény a tartalom keresési/kivitel

Problémák a tartalom keresési/kivitel nem minden adatvisszaadás bizonyos megfelelési biztonsági szűrő által adott Admin, és azt nem kommunikál a rendszergazdák minden beállítás volt lehetséges.

A probléma megoldásához ellenőrizze, hogy vannak-e bármilyen okozza-e a megfelelőség biztonsági szűrők:
1. Biztonsági és Megfelelési központba Powershell kapcsolódni
2. A következő parancsmagjaival futtatható:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org szervezet