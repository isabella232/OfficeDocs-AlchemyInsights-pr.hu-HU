---
title: Hiba a SpamHaus által blokkolt e-mail küldése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 52a5c20d59a2eac4c4bf465edaa888952d47f39f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387851"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>E-mail küldése a hiba: ügyfél-állomás segítségével Spamhaus blokkolva

Az IP-cím az üzenetet küldő tiltólistáján [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)tulajdonában van. Spamhaus blokkolja indokai feltört számlák megosztása a nyilvános IP-címet és az internetszolgáltató (ISP) házirendek gépek veszélybe. Lehetséges javításokat a következők:
  
- Blokkolt bejövő üzenetekhez az Office 365, ahol beállíthatja a forrás e-mail kiszolgálón szeretné okának és a blokk eltávolítása a Spamhaus webhelyről.

- Blokkolt bejövő üzenetekhez, ahol a forrás IP-cím tartozik valaki más Office 365 cím tulajdonosa szervizszerződésekből el kell távolítania a blokk a Spamhaus webhelyet. Ha az IP-címet a házirend blokk lista (PBL), a tulajdonos más statikus IP-cím, vagy távolítsa el a címet a PBL.

- A zárolt kimenő üzeneteket az Office 365 tartományból Ha az üzenetek útválasztása 3. fél szolgáltatáson keresztül kaphat Ez a hiba. A "WHOIS" keresési eszköz segítségével keresse meg a blokkolt IP cím tulajdonosa.
