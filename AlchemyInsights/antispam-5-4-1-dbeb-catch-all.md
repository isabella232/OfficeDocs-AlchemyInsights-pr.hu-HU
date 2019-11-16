---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672435"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="ee017-102">Fix szállítási problémák hibakódot 550 5.4.1 Relay hozzáférés megtagadva</span><span class="sxs-lookup"><span data-stu-id="ee017-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="ee017-103">Ez probléma előfordul mikor [korlátozás-hoz lát ha egy elektronikus levél cím van érvényes-hoz megakadályoz bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) Mikor tífusz a Hivatal 365 hálózat.</span><span class="sxs-lookup"><span data-stu-id="ee017-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="ee017-104">Próbálkozzon a következőkkel:</span><span class="sxs-lookup"><span data-stu-id="ee017-104">Try the following:</span></span>

1. <span data-ttu-id="ee017-105">Állapítsa meg, hogy a probléma egy teljes tartományra vagy egy e-mail címre vonatkozik-e:</span><span class="sxs-lookup"><span data-stu-id="ee017-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="ee017-106">Teljes tartomány: előfordul, hogy a tartományt szinkronizálni kell; megpróbál [elintézés a birtok-hoz belső aztán hát-hoz hiteles](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="ee017-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="ee017-107">Egy e-mail cím: előfordul, hogy a címet szinkronizálni kell; megváltozó a SMTP helyettes cím aztán megváltozó ez hát tud segít.</span><span class="sxs-lookup"><span data-stu-id="ee017-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="ee017-108">Állapítsa meg, hogy a probléma egy adott csoportra vagy nyilvános mappára vonatkozik-e.</span><span class="sxs-lookup"><span data-stu-id="ee017-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="ee017-109">Egyes objektumtípusok esetében előfordulhat, hogy a Azure Active Directory szolgáltatásban kézzel kell létrehozni az objektumokat.</span><span class="sxs-lookup"><span data-stu-id="ee017-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="ee017-110">Ha szüksége van további segítségre, kérjük, nyissa meg a támogatási jegyet, és adja meg a kérdés kiterjedését (includidng a típusú objektum te küldeni), hogy mi segítünk Önnek jobb.</span><span class="sxs-lookup"><span data-stu-id="ee017-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>