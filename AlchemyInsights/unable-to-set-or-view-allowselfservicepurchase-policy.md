---
title: Nem lehet beállítani vagy megtekinteni az AllowSelfServicePurchase házirendet
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826093"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nem lehet beállítani vagy megtekinteni az AllowSelfServicePurchase házirendet

Az AllowSelfServicePurchase házirend beállításakor vagy megtekintésekor a következő hibaüzenet jelenik meg:

*HandleError: Nem sikerült beolvasni a termék házirendet a PolicyId 'AllowSelfServicePurchase', ErrorMessage - A mögöttes kapcsolat lezárult: Váratlan hiba történt egy küldéskor.*

Ezt a Transport Layer Security (TLS) egy régebbi verziója okozhatja. Az MSCommerce szolgáltatás csatlakoztatásának 1.2-es vagy újabb TLS-et kell használnia.  

Az alábbi lépésekkel engedélyezze vagy állítsa a TLS protokollt 1.2-esre, ellenőrizze és próbálkozzon újra.
 1. A PowerShell parancssorában (PS C: a következő paranccsal állítsa a \) TLS protokollt az 1.2-es verzióra:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Ellenőrizze a használatban van TLS protokollokat az alábbi paranccsal:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Szükség szerint próbálja meg újból a Get vagy a Update parancsot.

