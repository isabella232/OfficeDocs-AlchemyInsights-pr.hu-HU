---
title: Hiba a SpamHaus által blokkolt e-mail küldésekor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714260"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Hiba az e-mail küldésekor: Az ügyfélállomás blokkolva van a Spamhaus használatával

Az üzenetet küldő IP-cím a [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)tulajdonában lévő tiltólistán található. A Spamhaus által letiltott okok közé tartoznak a feltört fiókok, a nyilvános IP-címet megosztó feltört gépek és az internetszolgáltatóra vonatkozó házirendek. A lehetséges javítások a következők:
  
- A blokkolt bejövő üzenetek, ahol ellenőrzik a forrás e-mail szerver, meg kell határoznia az okát, és távolítsa el a blokkot a Spamhaus honlapján.

- A blokkolt bejövő üzenetek esetében, ahol a forrás IP-cím valaki másé, a cím tulajdonosának el kell távolítania a blokkot a Spamhaus webhelyről. Ha az IP-cím szerepel a házirend-blokklistán (PBL), a tulajdonos másik statikus IP-címet rendelhet hozzá, vagy eltávolíthatja a címet a PBL-ből.

- A Microsofthoz csatlakoztatott tartományból letiltott kimenő üzenetek esetén ez a hibaüzenet akkor jelenhet meg, ha az üzenetek et egy külső szolgáltatáson keresztül továbbítják. A WHOIS kereséseszközével megkeresheti a blokkolt IP-cím tulajdonosát.
