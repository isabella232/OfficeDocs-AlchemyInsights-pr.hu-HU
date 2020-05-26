---
title: Segítségre van szüksége az e-mail küldési korlátokkal kapcsolatban?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357864"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="5aa61-102">Segítségre van szüksége az e-mail küldési korlátokkal kapcsolatban?</span><span class="sxs-lookup"><span data-stu-id="5aa61-102">Need help with email sending limits?</span></span>

<span data-ttu-id="5aa61-103">Az alábbiakban a **by-design küldési korlátok** a szolgáltatásban érvényesített.</span><span class="sxs-lookup"><span data-stu-id="5aa61-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="5aa61-104">Ezekről a korlátokról bővebben [itt](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)olvashat.</span><span class="sxs-lookup"><span data-stu-id="5aa61-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="5aa61-105">A kéretlen tömeges üzenetek kézbesítésének megakadályozása érdekében **felhasználónkénti címzetti díjkorlátokat**alkalmazunk az összes kimenő és belső üzenetre.</span><span class="sxs-lookup"><span data-stu-id="5aa61-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="5aa61-106">Az összes termékhelyesbben ez a korlát **naponta 10 000 címzettet.**</span><span class="sxs-lookup"><span data-stu-id="5aa61-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="5aa61-107">Azoknak az ügyfeleknek, akiknek jogos tömeges kereskedelmi e-maileket (például ügyfélhírleveleket) kell küldeniük, az ilyen szolgáltatásokra szakosodott külső szolgáltatókat kell használniuk.</span><span class="sxs-lookup"><span data-stu-id="5aa61-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="5aa61-108">**Megjegyzés:** A címzettségi sebesség korlátja elérése után az üzenetek nem küldhetők el a postaládából, amíg az elmúlt 24 órában küldött címzettek száma nem csökken a korlát alá.</span><span class="sxs-lookup"><span data-stu-id="5aa61-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="5aa61-109">A felhasználó addig nem tud üzeneteket küldeni.</span><span class="sxs-lookup"><span data-stu-id="5aa61-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="5aa61-110">A rendszer az összes ska-ra alkalmazza a **percenként 30** üzenetsebesség-korlátot.</span><span class="sxs-lookup"><span data-stu-id="5aa61-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="5aa61-111">Ez határozza meg, hogy a felhasználó hány üzenetet küldhet exchange online fiókjából egy adott időszakon belül.</span><span class="sxs-lookup"><span data-stu-id="5aa61-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="5aa61-112">A **Címzett, másolatot kap és titkos másolat mezőkben** az összes termékalkalmazáson keresztül engedélyezett címzettek maximális száma **1000 címzett.**</span><span class="sxs-lookup"><span data-stu-id="5aa61-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="5aa61-113">A korlát testreszabásához [itt](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)olvashat.</span><span class="sxs-lookup"><span data-stu-id="5aa61-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
