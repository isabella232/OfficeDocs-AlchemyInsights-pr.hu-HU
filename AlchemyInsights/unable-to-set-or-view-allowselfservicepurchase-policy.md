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
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020194"
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

