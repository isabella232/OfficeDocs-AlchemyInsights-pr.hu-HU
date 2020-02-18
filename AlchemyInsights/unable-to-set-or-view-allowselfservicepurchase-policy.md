---
title: Nem lehet beállítani vagy megtekinteni az AllowSelfServicePurchase házirendet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091714"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nem lehet beállítani vagy megtekinteni az AllowSelfServicePurchase házirendet

Az AllowSelfServicePurchase házirend beállításakor vagy megtekintésekor a következő hibaüzenet jelenik meg:

*HandleError : Nem sikerült beolvasni a PolicyId "AllowSelfServicePurchase" termékházirendjét, ErrorMessage - Az alapul szolgáló kapcsolat megszakadt: Váratlan hiba történt a küldéssorán.*

Ennek oka lehet a Transport Layer Security (TLS) régebbi verziója. Az MSCommerce szolgáltatás csatlakoztatásához a TLS 1.2-es vagy nagyobb at kell használnia.  

A TLS protokoll 1.2-es engedélyezéséhez/beállításához próbálkozzon az alábbi lépésekkel, ellenőrizze és próbálkozzon újra.
 1. A PowerShell parancssorába (PS C:\) írja be a következő parancsot a TLS protokoll 1.2-es verzióra való beállításához:

    \[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12

2. Ellenőrizze a használatban lévő TLS protokoll(oka)t a következő paranccsal:

    \[Net.ServicePointManager]::SecurityProtocol 

3. Próbálkozzon újra a Get vagy Update parancsokkal, ha szükséges.

