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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="1593f-102">E-mail-küldési hiba: a Spamhaus-on blokkolt ügyfélalkalmazás</span><span class="sxs-lookup"><span data-stu-id="1593f-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="1593f-103">Az üzenetet elküldő IP-cím egy [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)által birtokolt blokk listán található.</span><span class="sxs-lookup"><span data-stu-id="1593f-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="1593f-104">Az Spamhaus által letiltott fiókok közé tartozik a feltört fiókok, a nyilvános IP-címet és az internetszolgáltatót tartalmazó házirendek.</span><span class="sxs-lookup"><span data-stu-id="1593f-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="1593f-105">A lehetséges javítások a következők:</span><span class="sxs-lookup"><span data-stu-id="1593f-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="1593f-106">A forrás levelezési kiszolgáló felügyeletekor blokkolt bejövő üzenetek esetében meg kell határoznia az okát, és el kell távolítania a blokkot a Spamhaus webhelyről.</span><span class="sxs-lookup"><span data-stu-id="1593f-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="1593f-107">Azoknál a tiltott bejövő üzenetekben, amelyekben a forrás IP-címe valaki másnak tartozik, a cím tulajdonosa el kell távolítania a blokkot a Spamhaus webhelyről.</span><span class="sxs-lookup"><span data-stu-id="1593f-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="1593f-108">Ha az IP-cím a házirend-blokkoló listában (PBL) található, a tulajdonos rendelhet egy másik statikus IP-címet, vagy eltávolíthatja a címet a PBL.</span><span class="sxs-lookup"><span data-stu-id="1593f-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="1593f-109">Ha a tartományból letiltott kimenő üzeneteket a Microsofthoz kapcsolta, akkor a következő hibaüzenet jelenhet meg, ha az üzeneteket külső fél szolgáltatással irányítja át.</span><span class="sxs-lookup"><span data-stu-id="1593f-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="1593f-110">A letiltott IP-cím tulajdonosának megkereséséhez használhatja a WHOIS-kereső eszközt.</span><span class="sxs-lookup"><span data-stu-id="1593f-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
