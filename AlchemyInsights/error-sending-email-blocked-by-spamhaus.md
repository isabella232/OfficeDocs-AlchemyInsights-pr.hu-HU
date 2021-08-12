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
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946742"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>E-mail-küldési hiba: Az ügyfél gazdada blokkolva van a Spamhaus használatával

Az üzenetet küldő IP-cím szerepel a [Spamhaus egyik tiltólistán.](https://go.microsoft.com/fwlink/p/?linkid=123245) A Spamhaus többek között a következő okokból tilthatja le: feltört fiókok, nyilvános IP-címet megosztó feltört gépek és internetszolgáltatói házirendek. Lehetséges javítások:
  
- A blokkolt bejövő üzenetek esetén, ahol Ön ellenőrzi a forrás levelezőkiszolgálót, meg kell állapítania a letiltás okát, és el kell távolítania a Spamhaus webhelyén.

- A letiltott bejövő üzenetek esetén, amelyekben a forrás IP-cím valaki más tulajdonában van, a cím tulajdonosának el kell távolítania a tiltásokat a Spamhaus webhelyén. Ha az IP-cím szerepel a Policy Block List (PBL) listán, a tulajdonos másik statikus IP-címet rendelhet hozzá, vagy eltávolíthatja a címet a PBL listából.

- A Microsofthoz csatlakoztatott tartományból kimenő üzenetek esetén akkor jelenik meg ez a hibaüzenet, ha az üzeneteket egy külső szolgáltatáson keresztül irányítják át. A WHOIS keresési eszközzel megkeresheti a letiltott IP-cím tulajdonosát.
