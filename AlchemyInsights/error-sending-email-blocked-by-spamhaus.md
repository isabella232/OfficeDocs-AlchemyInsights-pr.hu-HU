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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="3b10b-102">Hiba az e-mail küldésekor: Az ügyfélállomás blokkolva van a Spamhaus használatával</span><span class="sxs-lookup"><span data-stu-id="3b10b-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="3b10b-103">Az üzenetet küldő IP-cím a [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)tulajdonában lévő tiltólistán található.</span><span class="sxs-lookup"><span data-stu-id="3b10b-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="3b10b-104">A Spamhaus által letiltott okok közé tartoznak a feltört fiókok, a nyilvános IP-címet megosztó feltört gépek és az internetszolgáltatóra vonatkozó házirendek.</span><span class="sxs-lookup"><span data-stu-id="3b10b-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="3b10b-105">A lehetséges javítások a következők:</span><span class="sxs-lookup"><span data-stu-id="3b10b-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="3b10b-106">A blokkolt bejövő üzenetek, ahol ellenőrzik a forrás e-mail szerver, meg kell határoznia az okát, és távolítsa el a blokkot a Spamhaus honlapján.</span><span class="sxs-lookup"><span data-stu-id="3b10b-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="3b10b-107">A blokkolt bejövő üzenetek esetében, ahol a forrás IP-cím valaki másé, a cím tulajdonosának el kell távolítania a blokkot a Spamhaus webhelyről.</span><span class="sxs-lookup"><span data-stu-id="3b10b-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="3b10b-108">Ha az IP-cím szerepel a házirend-blokklistán (PBL), a tulajdonos másik statikus IP-címet rendelhet hozzá, vagy eltávolíthatja a címet a PBL-ből.</span><span class="sxs-lookup"><span data-stu-id="3b10b-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="3b10b-109">A Microsofthoz csatlakoztatott tartományból letiltott kimenő üzenetek esetén ez a hibaüzenet akkor jelenhet meg, ha az üzenetek et egy külső szolgáltatáson keresztül továbbítják.</span><span class="sxs-lookup"><span data-stu-id="3b10b-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="3b10b-110">A WHOIS kereséseszközével megkeresheti a blokkolt IP-cím tulajdonosát.</span><span class="sxs-lookup"><span data-stu-id="3b10b-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
