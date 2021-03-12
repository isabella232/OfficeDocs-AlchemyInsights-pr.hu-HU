---
title: A TLS 1.0 és a TLS 1.1 letiltás miatt nem lehet e-maileket küldeni/fogadni az Office 365-be/
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
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745016"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>A TLS 1.0 és a TLS 1.1 letiltás miatt nem lehet e-maileket küldeni/fogadni az Office 365-be/

Amint azt az MC229914-et, a TLS 1.0-s és a TLS 1.1-es elavultást követő üzenetközpont is igazolta, az Exchange Online levélforgalom végpontjainak kényszerítését kezdték meg. Az Office 365 hamarosan nem fogadja el a külső forrásokból származó TLS 1.0-s és TLS 1.1-es e-mail-kapcsolatokat. Ezenkívül az Exchange Online soha nem használ TLS 1.0-s vagy 1.1-es portot a kimenő e-mailek küldését. Ha a TLS 1.0-s vagy 1.1-es letiltása miatt problémákat tapasztal, az alábbi hibaüzenetek egyikét tapasztalhatja:

- A feladó sikertelen kézbesítésről szóló jelentése visszapattan – '421 4.4.2 A Kapcsolat a SocketError miatt megszakadt'
- Hiba a helyszíni kiszolgáló Várólistás megjelenítőben, amely a Officer 365-nek küld e-mailt – '421 4.4.2 A SocketError miatt megszakadt a kapcsolat"
- A SocketError hiba [miatt](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) nem sikerült a TLS egyeztetése az Összekötők küldése naplóban a kiszolgálón, amely e-maileket küld az Office 365-be
- Hiba az Összekötők küldése és fogadása protokollnaplóban – '451 5.7.3 KEZDÉSI PARANCS ki kell adva'

Ha a fenti hibák bármelyikét tapasztalja, az alábbi beállításkulcsok ellenőrzésével győződjön meg arról, hogy a TLS 1.2 engedélyezve van a TLS 1.2-es kiszolgálón.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

Ha módosítja a fenti beállításkulcsokat a TLS 1.2 engedélyezéséhez, indítsa újra a kiszolgálót a módosítások érvénybe léptéhez. Ellenőrizze azt is, hogy telepítve vannak-e a Windows és az Exchange legújabb frissítései.

További információ:

- [Exchange Server TLS – útmutató, 1. rész: A TLS 1.2-es verziójának készült készülő része – Microsoft technikai közösség](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Az Exchange Server TLS 2. útmutatása: A TLS 1.2 engedélyezése és a nem használó ügyfelek azonosítása – Microsoft technikai közösség](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [A levelezési esetek ismertetése abban az esetben, ha nem lehet TLS-verziókat egyeztetni az Exchange Online-sal – Microsoft technikai közösség](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
