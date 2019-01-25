---
title: Hiba a SpamHaus által blokkolt e-mail küldése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473295"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>E-mail küldése a hiba: ügyfél-állomás segítségével Spamhaus blokkolva

Az IP-cím az üzenetet küldő tiltólistáján [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)tulajdonában van. Spamhaus blokkolja indokai feltört számlák megosztása a nyilvános IP-címet és az internetszolgáltató (ISP) házirendek gépek veszélybe. Lehetséges javításokat a következők:
  
- Blokkolt bejövő üzenetekhez az Office 365, ahol beállíthatja a forrás e-mail kiszolgálón szeretné okának és a blokk eltávolítása a Spamhaus webhelyről.
    
- Blokkolt bejövő üzenetekhez, ahol a forrás IP-cím tartozik valaki más Office 365 cím tulajdonosa szervizszerződésekből el kell távolítania a blokk a Spamhaus webhelyet. Ha az IP-címet a házirend blokk lista (PBL), a tulajdonos más statikus IP-cím, vagy távolítsa el a címet a PBL.
    
- A zárolt kimenő üzeneteket az Office 365 tartományból Ha az üzenetek útválasztása 3. fél szolgáltatáson keresztül kaphat Ez a hiba. A "WHOIS" keresési eszköz segítségével keresse meg a blokkolt IP cím tulajdonosa.
    

