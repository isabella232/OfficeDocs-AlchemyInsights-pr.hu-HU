---
title: Kimenő továbbítási készlet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381716"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="6a5a2-102">Kimenő továbbítási készlet</span><span class="sxs-lookup"><span data-stu-id="6a5a2-102">Outbound relay pool</span></span>

<span data-ttu-id="6a5a2-103">A Microsoft módosítja az e-mailek továbbításának vagy továbbításának beállításait a Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6a5a2-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="6a5a2-104">Bizonyos esetekben az üzeneteket egy speciális továbbítókészletet használva továbbítja vagy továbbítja Microsoft 365 keresztül a továbbításon keresztül.</span><span class="sxs-lookup"><span data-stu-id="6a5a2-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="6a5a2-105">A továbbítási készlet használatával küldött üzenetek a címzett levélszemétmappába kerülnek.</span><span class="sxs-lookup"><span data-stu-id="6a5a2-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="6a5a2-106">További információ: [Kimenő kézbesítési készletek](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="6a5a2-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="6a5a2-107">A továbbítási készlet használatával kapcsolatos esetek elkerülése érdekében győződjön meg arról, hogy a továbbított/továbbított üzenetek megfelelnek az alábbi feltételek egyikének:</span><span class="sxs-lookup"><span data-stu-id="6a5a2-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="6a5a2-108">A kimenő feladó a bérlő elfogadott tartománya.</span><span class="sxs-lookup"><span data-stu-id="6a5a2-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="6a5a2-109">A feladó házirend-keretrendszere (SPF) az üzenet be- vagy Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6a5a2-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="6a5a2-110">A P2 feladó tartományában a domainKeys Identified Mail (DKIM) tartománynév jelenik meg, amikor az üzenet Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6a5a2-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="6a5a2-111">A fenti feltételeknek megfelelő üzeneteket a rendszer nem továbbítja a továbbítási készleten keresztül.</span><span class="sxs-lookup"><span data-stu-id="6a5a2-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="6a5a2-112">Ha tartománya MX rekordja egy külső vagy helyszíni kiszolgálóra mutat, továbbfejlesztett szűrés használatával ellenőrizze, hogy helyes-e az SPF-ellenőrzés a bejövő e-maileknél, és hogy ne küldjön e-maileket a továbbítási készleten keresztül.</span><span class="sxs-lookup"><span data-stu-id="6a5a2-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="6a5a2-113">**Hogyan tudhatja meg, hogy hatással vannak-e a továbbítási készletre?**</span><span class="sxs-lookup"><span data-stu-id="6a5a2-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="6a5a2-114">Ha a továbbított vagy továbbított e-mailek a fenti feltételek valamelyikét használják, az üzenetek nem lesznek továbbítva a továbbítókészleten keresztül.</span><span class="sxs-lookup"><span data-stu-id="6a5a2-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="6a5a2-115">Ha azonban egy üzenet továbbítási készleten keresztül történik, a kimenő kiszolgáló IP-címe a 40.95.0.0/16 tartományba esik, és a kimenő kiszolgáló neve **rly** értékeket tartalmaz a névben.</span><span class="sxs-lookup"><span data-stu-id="6a5a2-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

