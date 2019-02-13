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
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912350"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>E-mail küldése a hiba: ügyfél-állomás segítségével Spamhaus blokkolva

Az IP-cím az üzenetet küldő tiltólistáján [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)tulajdonában van. Spamhaus blokkolja indokai feltört számlák megosztása a nyilvános IP-címet és az internetszolgáltató (ISP) házirendek gépek veszélybe. Lehetséges javításokat a következők:
  
- Blokkolt bejövő üzenetekhez az Office 365, ahol beállíthatja a forrás e-mail kiszolgálón szeretné okának és a blokk eltávolítása a Spamhaus webhelyről.
    
- Blokkolt bejövő üzenetekhez, ahol a forrás IP-cím tartozik valaki más Office 365 cím tulajdonosa szervizszerződésekből el kell távolítania a blokk a Spamhaus webhelyet. Ha az IP-címet a házirend blokk lista (PBL), a tulajdonos más statikus IP-cím, vagy távolítsa el a címet a PBL.
    
- A zárolt kimenő üzeneteket az Office 365 tartományból Ha az üzenetek útválasztása 3. fél szolgáltatáson keresztül kaphat Ez a hiba. A "WHOIS" keresési eszköz segítségével keresse meg a blokkolt IP cím tulajdonosa.
    

