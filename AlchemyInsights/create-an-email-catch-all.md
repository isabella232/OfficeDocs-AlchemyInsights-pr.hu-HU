---
title: E-mail-fogás létrehozása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712988"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="c0002-102">E-mail-fogás létrehozása</span><span class="sxs-lookup"><span data-stu-id="c0002-102">Create an email catch all</span></span>

<span data-ttu-id="c0002-103">Az összes fogás használata erősen ellenjavallt.</span><span class="sxs-lookup"><span data-stu-id="c0002-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="c0002-104">Jobb, ha vissza szeretne térni a feladónak, hogy a feladók megismerjék az üzenetét, hogy a címzettek ne legyenek kézbesítve, így elvégezhetik őket.</span><span class="sxs-lookup"><span data-stu-id="c0002-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="c0002-105">Úgy is korlátozhatja a figyelt postaládát, hogy csak a korábban érvényes e-mail-címeket kapja meg.</span><span class="sxs-lookup"><span data-stu-id="c0002-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="c0002-106">Bármely fogás minden postaládában sok levélszemét fog megjelenni, és előfordulhat, hogy végül nem figyeltek meg.</span><span class="sxs-lookup"><span data-stu-id="c0002-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="c0002-107">(Vannak fogadási korlátok.)</span><span class="sxs-lookup"><span data-stu-id="c0002-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="c0002-108">Ha úgy dönt, hogy továbblép, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="c0002-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="c0002-109">Hozzon létre egy dinamikus terjesztési csoportot, & a "minden címzett típusa" szó szerepel.</span><span class="sxs-lookup"><span data-stu-id="c0002-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="c0002-110">Hozzon létre egy dedikált postaládát az e-mailek elfogásához, például catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="c0002-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="c0002-111">Az adott tartomány esetében állítsa a DomainType a "InternalRelay" értékre.</span><span class="sxs-lookup"><span data-stu-id="c0002-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="c0002-112">Ha később eltávolítja az egész fogást, győződjön meg arról, hogy a tartomány vissza a mérvadó értékre van állítva.</span><span class="sxs-lookup"><span data-stu-id="c0002-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="c0002-113">Hozzon létre egy Hibaelhárítóhttps://configure.Office.com/scenario.aspx?SID=12 átviteli szabályt az alábbiak szerint:</span><span class="sxs-lookup"><span data-stu-id="c0002-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="c0002-114">Ha a feladó "a szervezeten kívül"</span><span class="sxs-lookup"><span data-stu-id="c0002-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="c0002-115">Az üzenet átirányítása a Catchall@domain.com-ra</span><span class="sxs-lookup"><span data-stu-id="c0002-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="c0002-116">Kivéve, ha a címzett a allusers@domain.com tagja (a terjesztési csoport az összes tagot tartalmazza)</span><span class="sxs-lookup"><span data-stu-id="c0002-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="c0002-117">Annak ellenőrzése, hogy az új postaládák hozzá lettek-e adva a dinamikus terjesztési csoporthoz</span><span class="sxs-lookup"><span data-stu-id="c0002-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
