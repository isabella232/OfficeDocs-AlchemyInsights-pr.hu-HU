---
title: Nem lehet e-maileket küldeni/fogadni Office 365 TLS 1.0-s és TLS 1.1-es letiltása miatt
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054908"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nem lehet e-maileket küldeni/fogadni Office 365 TLS 1.0-s és TLS 1.1-es letiltása miatt

Amint azt az MC229914-et, a TLS 1.0-s és a TLS 1.1-es elavultást követő üzenetközpont is megerősítette, az e-mail-forgalom végpontjainak Exchange Online kényszerítés. Hamarosan Office 365 külső forrásokból származó TLS 1.0-s és TLS 1.1-es e-mail-kapcsolatokat. Ezenkívül a Exchange Online a TLS 1.0-s vagy 1.1-es használatával küld kimenő e-maileket. Ha a TLS 1.0-s vagy 1.1-es letiltása miatt problémákat tapasztal, az alábbi hibaüzenetek egyikét tapasztalhatja:

- A feladó sikertelen kézbesítésről szóló jelentése visszapattan – '421 4.4.2 A Kapcsolat a SocketError miatt megszakadt'
- Hiba a helyszíni kiszolgáló Várólistás megjelenítőben, amely a Officer 365-nek küld e-mailt – '421 4.4.2 A SocketError miatt megszakadt a kapcsolat"
- A SocketError hiba [a](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) TLS Office 365 küldési kiszolgálón az Összekötő protokollok küldése naplójában
- Hiba az Összekötők küldése és fogadása protokollnaplóban – '451 5.7.3 KEZDÉSI PARANCS ki kell adva'

Ha a fenti hibák bármelyikét tapasztalja, az alábbi beállításkulcsok ellenőrzésével győződjön meg arról, hogy a TLS 1.2 engedélyezve van a TLS 1.2-es kiszolgálón.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

Ha módosítja a fenti beállításkulcsokat a TLS 1.2 engedélyezéséhez, indítsa újra a kiszolgálót a módosítások érvénybe léptéhez. Ellenőrizze azt is, hogy telepítve vannak-e a Windows és Exchange frissítések.

További információ:

- [Exchange Server TLS-útmutatás, 1. rész: A TLS 1.2-es verziójának használatba vennie – Microsoft technikai közösség](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server A TLS 2. útmutatása: A TLS 1.2 engedélyezése és a nem használó ügyfelek azonosítása – Microsoft technikai közösség](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [A levelezési esetek ismertetése abban az esetben, ha a TLS-verziókban nem lehet megegyezni a Exchange Online – Microsoft technikai közösség](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
