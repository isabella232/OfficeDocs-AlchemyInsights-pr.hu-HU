---
title: Tartalom keresés eredménye
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516781"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="18f96-102">Nincs eredmény a tartalom keresési/kivitel</span><span class="sxs-lookup"><span data-stu-id="18f96-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="18f96-103">Problémák a tartalom keresési/kivitel nem minden adatvisszaadás bizonyos megfelelési biztonsági szűrő által adott Admin, és azt nem kommunikál a rendszergazdák minden beállítás volt lehetséges.</span><span class="sxs-lookup"><span data-stu-id="18f96-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="18f96-104">A probléma megoldásához ellenőrizze, hogy vannak-e bármilyen okozza-e a megfelelőség biztonsági szűrők:</span><span class="sxs-lookup"><span data-stu-id="18f96-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="18f96-105">Biztonsági és Megfelelési központba Powershell kapcsolódni</span><span class="sxs-lookup"><span data-stu-id="18f96-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="18f96-106">A következő parancsmagjaival futtatható:</span><span class="sxs-lookup"><span data-stu-id="18f96-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="18f96-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="18f96-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="18f96-108">Get-ComplianceSecurityFilter-$org szervezet</span><span class="sxs-lookup"><span data-stu-id="18f96-108">Get-ComplianceSecurityFilter -Organization $org</span></span>