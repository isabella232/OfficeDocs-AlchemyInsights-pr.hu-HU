---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821449"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="7a264-102">Az 550 5.4.1-es hibakódú továbbítási hozzáférés megtagadva kézbesítési problémáinak megoldása</span><span class="sxs-lookup"><span data-stu-id="7a264-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="7a264-103">Ez a [](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) probléma akkor jelentkezik, amikor ellenőrzi, hogy érvényes-e egy e-mail-cím, hogy megakadályozza a visszapattanásokat a Microsoft-hálózatba való belépéskor.</span><span class="sxs-lookup"><span data-stu-id="7a264-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="7a264-104">Próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="7a264-104">Try the following:</span></span>

1. <span data-ttu-id="7a264-105">Annak megállapítása, hogy a probléma egy teljes tartományra vagy egyetlen e-mail-címre jellemző-e:</span><span class="sxs-lookup"><span data-stu-id="7a264-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="7a264-106">A teljes tartomány: Időnként előfordulhat, hogy szinkronizálni kell a tartományt; próbálja [meg a tartományt Belső, majd vissza a Mérvadó beállításra.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="7a264-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="7a264-107">Egyetlen e-mail-cím: Néha szinkronizálni kell a címet; az smtp-proxycím módosítása, majd visszaváltása segíthet.</span><span class="sxs-lookup"><span data-stu-id="7a264-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="7a264-108">Állapítsa meg, hogy a probléma csoportra vagy nyilvános mappára jellemző-e.</span><span class="sxs-lookup"><span data-stu-id="7a264-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="7a264-109">Egyes objektumtípusok esetében az objektumokat manuálisan kell létrehozni az Azure Active Directoryban.</span><span class="sxs-lookup"><span data-stu-id="7a264-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="7a264-110">Ha további segítségre van szüksége, nyisson egy támogatási jegyet, és adja meg a probléma hatókörét (beleértve a küldeni kívánt objektum típusát), hogy jobban segítsünk Önnek.</span><span class="sxs-lookup"><span data-stu-id="7a264-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>