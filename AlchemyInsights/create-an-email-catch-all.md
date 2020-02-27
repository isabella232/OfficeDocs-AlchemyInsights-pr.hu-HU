---
title: Hozzon létre egy e-mail fogás az összes
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286195"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="00fb9-102">Hozzon létre egy e-mail fogás az összes</span><span class="sxs-lookup"><span data-stu-id="00fb9-102">Create an email catch all</span></span>

<span data-ttu-id="00fb9-103">Használata a fogás minden erősen ellenszegül.</span><span class="sxs-lookup"><span data-stu-id="00fb9-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="00fb9-104">Sokkal jobb, hogy egy visszapattanó vissza a feladó tudatja, hogy az üzenetet nem lehet kézbesíteni a címzett, így azok lépéseket.</span><span class="sxs-lookup"><span data-stu-id="00fb9-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="00fb9-105">A figyelt postaládát úgy is korlátozhatja, hogy csak a korábban érvényes e-mail-címek foghatók.</span><span class="sxs-lookup"><span data-stu-id="00fb9-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="00fb9-106">Minden fogás minden postaláda kap egy jó adag spam, és végül töltse ki, ha nem szorosan figyelemmel kíséri.</span><span class="sxs-lookup"><span data-stu-id="00fb9-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="00fb9-107">(Vannak fogadási korlátok.)</span><span class="sxs-lookup"><span data-stu-id="00fb9-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="00fb9-108">Ha úgy dönt, hogy folytatja, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="00fb9-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="00fb9-109">Hozzon létre egy dinamikus terjesztési csoportot, & tartalmazza a "Minden címzett típusa" című &.</span><span class="sxs-lookup"><span data-stu-id="00fb9-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="00fb9-110">Hozzon létre egy dedikált postaládát az e-mailek, például a catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="00fb9-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="00fb9-111">Az adott tartományhoz állítsa a DomainType programot "InternalRelay" beállításra.</span><span class="sxs-lookup"><span data-stu-id="00fb9-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="00fb9-112">Ha később eltávolítja az összes fogást, állítsa vissza a tartományt Mérvadó szintre.</span><span class="sxs-lookup"><span data-stu-id="00fb9-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="00fb9-113">Hozzon létre egy Mailflow átviteli szabályt az alábbiak szerint:</span><span class="sxs-lookup"><span data-stu-id="00fb9-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="00fb9-114">Ha a feladó "szervezeten kívül"</span><span class="sxs-lookup"><span data-stu-id="00fb9-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="00fb9-115">Az üzenet átirányítása Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="00fb9-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="00fb9-116">Kivéve, ha a címzett tagja a allusers@domain.com (Distribution Group tartalmazza az összes tagja)</span><span class="sxs-lookup"><span data-stu-id="00fb9-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="00fb9-117">Annak ellenőrzése, hogy új postaládák kerültek-e a dinamikus terjesztési csoportba</span><span class="sxs-lookup"><span data-stu-id="00fb9-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
