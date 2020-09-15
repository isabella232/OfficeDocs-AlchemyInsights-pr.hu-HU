---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717363"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="ca034-102">A 550 5.4.1-es hibakódok kézbesítési hibáinak elhárítása a hozzáférés megtagadásához</span><span class="sxs-lookup"><span data-stu-id="ca034-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="ca034-103">Ez a probléma akkor jelentkezik, ha [ellenőrzi, hogy egy e-mail-cím érvényes-e a bouncebacks megakadályozására](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) a Microsoft-hálózat beírásakor.</span><span class="sxs-lookup"><span data-stu-id="ca034-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="ca034-104">Próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="ca034-104">Try the following:</span></span>

1. <span data-ttu-id="ca034-105">Annak megállapítása, hogy a probléma egy teljes tartományra vagy egyetlen e-mail-címre vonatkozik-e:</span><span class="sxs-lookup"><span data-stu-id="ca034-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="ca034-106">Teljes tartomány: időnként a tartományt szinkronizálni kell; Próbálkozzon [a tartomány belső értékre állításával, majd vissza a mérvadó](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)értékre.</span><span class="sxs-lookup"><span data-stu-id="ca034-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="ca034-107">Egyetlen e-mail-cím: időnként szinkronizálni kell a címet. Ha módosítja az SMTP-proxy címét, majd újra módosítja, akkor segíthet.</span><span class="sxs-lookup"><span data-stu-id="ca034-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="ca034-108">Annak megállapítása, hogy a probléma egy csoportra vagy nyilvános mappára jellemző-e.</span><span class="sxs-lookup"><span data-stu-id="ca034-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="ca034-109">Egyes objektumtípusok esetén előfordulhat, hogy az Azure Active Directoryban manuálisan kell létrehozni az objektumokat.</span><span class="sxs-lookup"><span data-stu-id="ca034-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="ca034-110">Ha további segítségre van szüksége, nyisson meg egy támogatási jegyet, és adja meg a probléma hatókörét (többek között a küldendő objektum típusát is), így jobban segíthetünk.</span><span class="sxs-lookup"><span data-stu-id="ca034-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>