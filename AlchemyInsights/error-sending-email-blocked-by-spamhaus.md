---
title: Hiba a SpamHaus által letiltott e-mailek küldésekor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783805"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>E-mail-küldési hiba: a Spamhaus-on blokkolt ügyfélalkalmazás

Az üzenetet elküldő IP-cím egy [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)által birtokolt blokk listán található. Az Spamhaus által letiltott fiókok közé tartozik a feltört fiókok, a nyilvános IP-címet és az internetszolgáltatót tartalmazó házirendek. A lehetséges javítások a következők:
  
- A forrás levelezési kiszolgáló felügyeletekor blokkolt bejövő üzenetek esetében meg kell határoznia az okát, és el kell távolítania a blokkot a Spamhaus webhelyről.

- Azoknál a tiltott bejövő üzenetekben, amelyekben a forrás IP-címe valaki másnak tartozik, a cím tulajdonosa el kell távolítania a blokkot a Spamhaus webhelyről. Ha az IP-cím a házirend-blokkoló listában (PBL) található, a tulajdonos rendelhet egy másik statikus IP-címet, vagy eltávolíthatja a címet a PBL.

- Ha a tartományból letiltott kimenő üzeneteket a Microsofthoz kapcsolta, akkor a következő hibaüzenet jelenhet meg, ha az üzeneteket külső fél szolgáltatással irányítja át. A letiltott IP-cím tulajdonosának megkereséséhez használhatja a WHOIS-kereső eszközt.
