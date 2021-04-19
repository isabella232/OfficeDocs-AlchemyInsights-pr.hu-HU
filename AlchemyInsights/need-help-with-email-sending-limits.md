---
title: Segítségre van szüksége az e-mailek küldésének korlátozásával?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836281"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="fb1dd-102">Segítségre van szüksége az e-mailek küldésének korlátozásával?</span><span class="sxs-lookup"><span data-stu-id="fb1dd-102">Need help with email sending limits?</span></span>

<span data-ttu-id="fb1dd-103">Az alábbiakban a szolgáltatásban kényszerített **tervezés szerinti küldési korlátokat** ismerheti meg.</span><span class="sxs-lookup"><span data-stu-id="fb1dd-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="fb1dd-104">Ezekről a korlátozásokról további információt [itt talál](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="fb1dd-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="fb1dd-105">A kéretlen tömeges üzenetek kézbesítésének visszaszorítása érdekében felhasználónkénti **címzettarányos korlátokat alkalmazunk minden kimenő és belső üzenetre**.</span><span class="sxs-lookup"><span data-stu-id="fb1dd-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="fb1dd-106">Ez a korlát az összes termékváltozatban **10 000 címzett naponta**.</span><span class="sxs-lookup"><span data-stu-id="fb1dd-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="fb1dd-107">Azok az ügyfelek, akiknek valódi tömeges kereskedelmi e-mailt (például hírleveleket az ügyfeleknek) kell küldeniük, az e szolgáltatásokra specializálódott külső szolgáltatókat kell igénybe venniük.</span><span class="sxs-lookup"><span data-stu-id="fb1dd-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="fb1dd-108">**Megjegyzés**: Miután elérte a címzettek arányának korlátját, a rendszer nem tud üzenetet küldeni a postaládából, amíg a korlát alá nem esik azoknak a címzetteknek a száma, akiknek az elmúlt 24 órában üzenetet küldött.</span><span class="sxs-lookup"><span data-stu-id="fb1dd-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="fb1dd-109">A felhasználó csak ezt a pontot elérve tud majd üzeneteket küldeni.</span><span class="sxs-lookup"><span data-stu-id="fb1dd-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="fb1dd-110">A rendszer a **percenkénti 30 üzenet** üzenetarány-korlátot alkalmazza az összes termékváltozat esetén.</span><span class="sxs-lookup"><span data-stu-id="fb1dd-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="fb1dd-111">Ez meghatározza, hogy egy felhasználó hány üzenetet küldhet egy megadott időszakon belül az Exchange Online-fiókjából.</span><span class="sxs-lookup"><span data-stu-id="fb1dd-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="fb1dd-112">A **Címzett, Másolatot kap és Titkos másolat mezőben engedélyezett címzettek maximális száma** az összes termékváltozatban egyetlen e-mail esetén **1000 címzett** lehet.</span><span class="sxs-lookup"><span data-stu-id="fb1dd-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="fb1dd-113">A korlát testreszabásához [lépjen ide](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="fb1dd-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
