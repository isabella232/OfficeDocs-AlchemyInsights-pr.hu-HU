---
title: Nem lehet beállítani vagy megtekinteni a AllowSelfServicePurchase házirendjét
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735201"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nem lehet beállítani vagy megtekinteni a AllowSelfServicePurchase házirendjét

A AllowSelfServicePurchase házirend beállításakor vagy megtekintésekor a következő hibaüzenet jelenik meg:

*HandleError: nem sikerült lekérdezni a termékkulcsot a PolicyId "AllowSelfServicePurchase" ErrorMessage – az alapul szolgáló kapcsolat bezárult: váratlan hiba történt a küldéskor.*

Ennek oka az lehet, hogy a Transport Layer Security (TLS) régebbi verziójával rendelkezik. A MSCommerce szolgáltatás csatlakoztatásához TLS 1,2 vagy újabbt kell használnia.  

A következő lépésekkel engedélyezheti/állíthatja be a TLS-protokollt a 1,2-ra, az ellenőrzésre és az újrapróbálkozásra.
 1. A PowerShell parancssorába (PS C: \) írja be a következő parancsot a 1,2-es verzió TLS-protokolljának beállításához:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Ellenőrizze a használatban lévő TLS protokollt (ka) t, a következő paranccsal:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Szükség esetén próbálkozzon újra a Get vagy a Update parancs segítségével.

