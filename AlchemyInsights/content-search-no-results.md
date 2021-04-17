---
title: Nincs találat a tartalomkeresésben
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816850"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="ef89f-102">Nincs találat a tartalomkeresésből/-exportálásból</span><span class="sxs-lookup"><span data-stu-id="ef89f-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="ef89f-103">A tartalomkereséssel/-exportálással kapcsolatos problémákat az adott rendszergazda által megadott megfelelőségi biztonsági szűrő miatt lehet, amely nem adja vissza az adatokat az összes rendszergazdának.</span><span class="sxs-lookup"><span data-stu-id="ef89f-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="ef89f-104">A probléma megoldásához ellenőrizze, hogy vannak-e olyan megfelelőségi biztonsági szűrők, amelyek ezt okozhatják:</span><span class="sxs-lookup"><span data-stu-id="ef89f-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="ef89f-105">Csatlakozás a Biztonsági és megfelelőségi központ Powershell-parancshoz</span><span class="sxs-lookup"><span data-stu-id="ef89f-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="ef89f-106">Futtassa az alábbi parancsmagokat:</span><span class="sxs-lookup"><span data-stu-id="ef89f-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="ef89f-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="ef89f-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="ef89f-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="ef89f-108">Get-ComplianceSecurityFilter -Organization $org</span></span>