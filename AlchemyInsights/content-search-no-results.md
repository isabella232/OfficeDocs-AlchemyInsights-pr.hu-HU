---
title: Tartalmi találatok száma
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680649"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="4290d-102">A tartalom keresésének/exportálásának eredménye</span><span class="sxs-lookup"><span data-stu-id="4290d-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="4290d-103">A tartalmi kereséssel/exportálással kapcsolatos problémák oka az lehet, hogy bizonyos megfelelőségi biztonsági szűrőket egy bizonyos rendszergazdák állítanak be, és nem kommunikálnak a rendszergazdákkal.</span><span class="sxs-lookup"><span data-stu-id="4290d-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="4290d-104">A probléma megoldásához győződjön meg arról, hogy vannak-e olyan megfelelőségi biztonsági szűrők, amelyek az alábbi esetekben lehetnek így:</span><span class="sxs-lookup"><span data-stu-id="4290d-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="4290d-105">Csatlakozás a biztonsági és megfelelőségi központ Powershellhez</span><span class="sxs-lookup"><span data-stu-id="4290d-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="4290d-106">Futtassa az alábbi parancsmaggal található:</span><span class="sxs-lookup"><span data-stu-id="4290d-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="4290d-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="4290d-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="4290d-108">Get-ComplianceSecurityFilter-szervezet $org</span><span class="sxs-lookup"><span data-stu-id="4290d-108">Get-ComplianceSecurityFilter -Organization $org</span></span>