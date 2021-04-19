---
title: Segítségre van szüksége az e-mail küldési korlátozásokkal?
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
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="27b8d-102">Segítségre van szüksége az e-mail küldési korlátozásokkal?</span><span class="sxs-lookup"><span data-stu-id="27b8d-102">Need help with email sending limits?</span></span>

<span data-ttu-id="27b8d-103">Az alábbiakban **a szolgáltatásban kényszerített** küldési korlátozásokat olvashatja.</span><span class="sxs-lookup"><span data-stu-id="27b8d-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="27b8d-104">Ezekről a korlátokról itt található további [információ.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)</span><span class="sxs-lookup"><span data-stu-id="27b8d-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="27b8d-105">A kéretlen tömeges üzenetek kézbesítésének ellen érdekében felhasználóinkénti címzettdíj-korlátozásokat alkalmazunk minden kimenő és **belső üzenetre.**</span><span class="sxs-lookup"><span data-stu-id="27b8d-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="27b8d-106">Ez a korlát minden sususban **napi 10 000 címzettre van korlátozva.**</span><span class="sxs-lookup"><span data-stu-id="27b8d-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="27b8d-107">Az e szolgáltatásokra speciális külső szolgáltatókat kell használniuk azok az ügyfelek, akiknek valódi tömeges kereskedelmi e-maileket kell küldenie (például ügyfél hírleveleket).</span><span class="sxs-lookup"><span data-stu-id="27b8d-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="27b8d-108">**Megjegyzés:** A címzettek számának korlátjának elérése után a postaládából csak akkor lehet üzeneteket küldeni, ha az elmúlt 24 órában küldött címzettek száma nem csökken a korlátnál.</span><span class="sxs-lookup"><span data-stu-id="27b8d-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="27b8d-109">A felhasználó addig nem fog tudni üzeneteket küldeni.</span><span class="sxs-lookup"><span data-stu-id="27b8d-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="27b8d-110">Az üzenetek **percenkénti 30 üzenetre** vonatkozó korlátja minden sususra érvényes.</span><span class="sxs-lookup"><span data-stu-id="27b8d-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="27b8d-111">Ez azt határozza meg, hogy egy felhasználó hány üzenetet küldhet az Exchange Online-fiókjából a megadott időszakon belül.</span><span class="sxs-lookup"><span data-stu-id="27b8d-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="27b8d-112">Egy **e-mail Címzett,** Másolatot kap és Titkos másolat mezőjében legfeljebb **1000** címzett lehet.</span><span class="sxs-lookup"><span data-stu-id="27b8d-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="27b8d-113">A korlát testreszabásához itt [hatja meg a beállításokat.](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)</span><span class="sxs-lookup"><span data-stu-id="27b8d-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
