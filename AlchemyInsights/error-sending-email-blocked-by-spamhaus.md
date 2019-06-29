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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="661fd-102">E-mail küldése a hiba: ügyfél-állomás segítségével Spamhaus blokkolva</span><span class="sxs-lookup"><span data-stu-id="661fd-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="661fd-103">Az IP-cím az üzenetet küldő tiltólistáján [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)tulajdonában van.</span><span class="sxs-lookup"><span data-stu-id="661fd-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="661fd-104">Spamhaus blokkolja indokai feltört számlák megosztása a nyilvános IP-címet és az internetszolgáltató (ISP) házirendek gépek veszélybe.</span><span class="sxs-lookup"><span data-stu-id="661fd-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="661fd-105">Lehetséges javításokat a következők:</span><span class="sxs-lookup"><span data-stu-id="661fd-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="661fd-106">Blokkolt bejövő üzenetekhez az Office 365, ahol beállíthatja a forrás e-mail kiszolgálón szeretné okának és a blokk eltávolítása a Spamhaus webhelyről.</span><span class="sxs-lookup"><span data-stu-id="661fd-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="661fd-107">Blokkolt bejövő üzenetekhez, ahol a forrás IP-cím tartozik valaki más Office 365 cím tulajdonosa szervizszerződésekből el kell távolítania a blokk a Spamhaus webhelyet.</span><span class="sxs-lookup"><span data-stu-id="661fd-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="661fd-108">Ha az IP-címet a házirend blokk lista (PBL), a tulajdonos más statikus IP-cím, vagy távolítsa el a címet a PBL.</span><span class="sxs-lookup"><span data-stu-id="661fd-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="661fd-109">A zárolt kimenő üzeneteket az Office 365 tartományból Ha az üzenetek útválasztása 3. fél szolgáltatáson keresztül kaphat Ez a hiba.</span><span class="sxs-lookup"><span data-stu-id="661fd-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="661fd-110">A "WHOIS" keresési eszköz segítségével keresse meg a blokkolt IP cím tulajdonosa.</span><span class="sxs-lookup"><span data-stu-id="661fd-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
