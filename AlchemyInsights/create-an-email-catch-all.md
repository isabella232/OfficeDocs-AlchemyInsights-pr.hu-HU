---
title: Az összes e-mail fogó létrehozása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816202"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="30181-102">Az összes e-mail fogó létrehozása</span><span class="sxs-lookup"><span data-stu-id="30181-102">Create an email catch all</span></span>

<span data-ttu-id="30181-103">A minden kifogó használata kifejezetten ellenzi ezt.</span><span class="sxs-lookup"><span data-stu-id="30181-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="30181-104">Jobb, ha visszapattan a feladóhoz, és tudatja a feladóval, hogy az üzenetet nem lehetett címzettként kézbesíteni, hogy meg tudjanak oldani a lépéseket.</span><span class="sxs-lookup"><span data-stu-id="30181-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="30181-105">A figyelt postaládát úgy is korlátozhatja, hogy csak a korábban érvényes e-mail-címeket elfogja.</span><span class="sxs-lookup"><span data-stu-id="30181-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="30181-106">Minden elfogható postaláda sok levélszemetet kap, és végül kitöltheti őket, ha nem figyelik rendszeresen.</span><span class="sxs-lookup"><span data-stu-id="30181-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="30181-107">(Vannak fogadási korlátozások.)</span><span class="sxs-lookup"><span data-stu-id="30181-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="30181-108">Ha a folytatásról dönt, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="30181-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="30181-109">Dinamikus terjesztési csoport létrehozása & "Minden címzetttípus" gombra.</span><span class="sxs-lookup"><span data-stu-id="30181-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="30181-110">Létrehozhat egy dedikált postaládát az e-mailek (például e-mailek) catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="30181-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="30181-111">Az adott tartományhoz állítsa a DomainType tulajdonságot "InternalRelay" (Belső átfedés) beállításra.</span><span class="sxs-lookup"><span data-stu-id="30181-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="30181-112">Ha később eltávolítja a "Minden" halmazt, állítsa vissza a tartományt Mérvadóra.</span><span class="sxs-lookup"><span data-stu-id="30181-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="30181-113">Hozzon létre egy levélcsordulási átviteli szabályt az alábbiak szerint:</span><span class="sxs-lookup"><span data-stu-id="30181-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="30181-114">Ha a Feladó "Szervezeten kívül"</span><span class="sxs-lookup"><span data-stu-id="30181-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="30181-115">Az üzenet átirányítása a Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="30181-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="30181-116">Kivéve, ha a címzett tagja az allusers@domain.com (a terjesztési csoport az összes tagot tartalmazza)</span><span class="sxs-lookup"><span data-stu-id="30181-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="30181-117">Ellenőrizze, hogy az új postaládák bekerülnek-e a dinamikus terjesztési csoportba</span><span class="sxs-lookup"><span data-stu-id="30181-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
