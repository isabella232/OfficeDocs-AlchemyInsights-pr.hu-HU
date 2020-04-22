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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707913"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="803b4-102">Az 550 5.4.1-es hibakódú kézbesítési problémák megoldásának megoldása megtagadva</span><span class="sxs-lookup"><span data-stu-id="803b4-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="803b4-103">Ez a probléma akkor fordul [elő, ha ellenőrzi, hogy érvényes-e egy e-mail cím, hogy megakadályozza a visszapattanásokat](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) a Microsoft-hálózatba való belépéskor.</span><span class="sxs-lookup"><span data-stu-id="803b4-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="803b4-104">Próbálkozzon a következőkkel:</span><span class="sxs-lookup"><span data-stu-id="803b4-104">Try the following:</span></span>

1. <span data-ttu-id="803b4-105">Határozza meg, hogy a probléma egy teljes tartományra vagy egyetlen e-mail címre vonatkozik-e:</span><span class="sxs-lookup"><span data-stu-id="803b4-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="803b4-106">Teljes tartomány: Néha a tartományt szinkronizálni kell; próbálja meg [a tartományt Belső, majd vissza mérvadó ra.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="803b4-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="803b4-107">Egyetlen e-mail cím: Néha a címet szinkronizálni kell; megváltoztatása smtp proxy címét, majd megváltoztatja vissza segíthet.</span><span class="sxs-lookup"><span data-stu-id="803b4-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="803b4-108">Határozza meg, hogy a probléma egy csoportra vagy nyilvános mappára vonatkozik-e.</span><span class="sxs-lookup"><span data-stu-id="803b4-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="803b4-109">Bizonyos objektumtípusok esetében előfordulhat, hogy az objektumokat manuálisan kell létrehozni az Azure Active Directoryban.</span><span class="sxs-lookup"><span data-stu-id="803b4-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="803b4-110">Ha további segítségre van szüksége, nyisson meg egy támogatási jegyet, és adja meg a probléma hatókörét (beleértve az elküldött objektum típusát is), hogy jobban segíthessünk Önnek.</span><span class="sxs-lookup"><span data-stu-id="803b4-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>