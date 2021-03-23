---
title: Védelem a Backscatter-támadások ellen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036073"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="a09ed-102">Védelem a Backscatter-támadások ellen</span><span class="sxs-lookup"><span data-stu-id="a09ed-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="a09ed-103">A Visszapattanópata az el nem küldött üzenetekről kapott nem kézbesítésről szóló jelentések (más néven a kézbesítésről szóló jelentések vagy visszapattanó üzenetek).</span><span class="sxs-lookup"><span data-stu-id="a09ed-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="a09ed-104">A levélszemétküldők megfedik (hamisják) az üzeneteik **From:** címét, és gyakran valódi e-mail-címekkel adnak hitelességet az üzeneteikben.</span><span class="sxs-lookup"><span data-stu-id="a09ed-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="a09ed-105">Ha tehát a levélszemétküldők elkerülhetetlenül küldenek üzeneteket nem létező címzetteknek, a cél levelezési kiszolgálót lényegében átveszi a rendszer arra, hogy kézbesíthetetlen üzenetet küldjenek vissza egy sikertelen kézbesítésről szóló jelentésből a **feladói** cím hamis feladójának.</span><span class="sxs-lookup"><span data-stu-id="a09ed-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="a09ed-106">További információt az [EOP Backscatter szolgáltatásában talál.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)</span><span class="sxs-lookup"><span data-stu-id="a09ed-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="a09ed-107">**A Visszakattoló elleni védelem engedélyezése**</span><span class="sxs-lookup"><span data-stu-id="a09ed-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="a09ed-108">A Backscatter-védelem engedélyezéséhez kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="a09ed-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="a09ed-109">**protection.office.com > Threat Management > Policy > Antispam > Válassza a Levélszemétszűrő házirend és a Házirend szerkesztése > Levélszemét tulajdonságai > Megjelölés levélszemétként > sikertelen kézbesítésről szóló jelentés visszacsatoló levélszemétje > Beállítás "Be" beállításra**</span><span class="sxs-lookup"><span data-stu-id="a09ed-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="a09ed-110">Ha úgy véli, hogy feltörték a fiókját, tekintse át az alábbi információkat:</span><span class="sxs-lookup"><span data-stu-id="a09ed-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="a09ed-111">Válasz feltört e-mail-fiókra</span><span class="sxs-lookup"><span data-stu-id="a09ed-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="a09ed-112">Letiltott felhasználók eltávolítása az Office 365 Korlátozott felhasználók portálján</span><span class="sxs-lookup"><span data-stu-id="a09ed-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



