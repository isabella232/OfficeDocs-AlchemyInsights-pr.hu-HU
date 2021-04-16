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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="220d9-102">E-mail-küldési hiba: Az ügyfél gazdada blokkolva van a Spamhaus használatával</span><span class="sxs-lookup"><span data-stu-id="220d9-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="220d9-103">Az üzenetet küldő IP-cím szerepel a [Spamhaus egyik tiltólistán.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="220d9-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="220d9-104">A Spamhaus többek között a következő okokból tilthatja le: feltört fiókok, nyilvános IP-címet megosztó feltört gépek és internetszolgáltatói házirendek.</span><span class="sxs-lookup"><span data-stu-id="220d9-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="220d9-105">Lehetséges javítások:</span><span class="sxs-lookup"><span data-stu-id="220d9-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="220d9-106">A blokkolt bejövő üzenetek esetén, ahol Ön ellenőrzi a forrás levelezőkiszolgálót, meg kell állapítania a letiltás okát, és el kell távolítania a Spamhaus webhelyén.</span><span class="sxs-lookup"><span data-stu-id="220d9-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="220d9-107">A letiltott bejövő üzenetek esetén, amelyekben a forrás IP-cím valaki más tulajdonában van, a cím tulajdonosának el kell távolítania a tiltásokat a Spamhaus webhelyén.</span><span class="sxs-lookup"><span data-stu-id="220d9-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="220d9-108">Ha az IP-cím szerepel a Policy Block List (PBL) listán, a tulajdonos másik statikus IP-címet rendelhet hozzá, vagy eltávolíthatja a címet a PBL listából.</span><span class="sxs-lookup"><span data-stu-id="220d9-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="220d9-109">A Microsofthoz csatlakoztatott tartományból kimenő üzenetek esetén akkor jelenik meg ez a hibaüzenet, ha az üzeneteket egy külső szolgáltatáson keresztül irányítják át.</span><span class="sxs-lookup"><span data-stu-id="220d9-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="220d9-110">A WHOIS keresési eszközzel megkeresheti a letiltott IP-cím tulajdonosát.</span><span class="sxs-lookup"><span data-stu-id="220d9-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
