---
title: Hiba a SpamHaus által blokkolt e-mailek küldésekor
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813726"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>E-mail-küldési hiba: Az ügyfél gazdada blokkolva van a Spamhaus használatával

Az üzenetet küldő IP-cím szerepel a [Spamhaus egyik tiltólistán.](https://go.microsoft.com/fwlink/p/?linkid=123245) A Spamhaus többek között a következő okokból tilthatja le: feltört fiókok, nyilvános IP-címet megosztó feltört gépek és internetszolgáltatói házirendek. Lehetséges javítások:
  
- A blokkolt bejövő üzenetek esetén, ahol Ön ellenőrzi a forrás levelezőkiszolgálót, meg kell állapítania a letiltás okát, és el kell távolítania a Spamhaus webhelyén.

- A letiltott bejövő üzenetek esetén, amelyekben a forrás IP-cím valaki más tulajdonában van, a cím tulajdonosának el kell távolítania a tiltásokat a Spamhaus webhelyén. Ha az IP-cím szerepel a Policy Block List (PBL) listán, a tulajdonos másik statikus IP-címet rendelhet hozzá, vagy eltávolíthatja a címet a PBL listából.

- A Microsofthoz csatlakoztatott tartományból kimenő üzenetek esetén akkor jelenik meg ez a hibaüzenet, ha az üzeneteket egy külső szolgáltatáson keresztül irányítják át. A WHOIS keresési eszközzel megkeresheti a letiltott IP-cím tulajdonosát.
