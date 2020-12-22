---
title: A tartalom keresése/exportálása során a találatok között nincs eredmény
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727225"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="49146-102">A tartalom keresése/exportálása során a találatok között nincs eredmény</span><span class="sxs-lookup"><span data-stu-id="49146-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="49146-103">Ha problémák lépnek fel a következő eDiscovery-esetekben:</span><span class="sxs-lookup"><span data-stu-id="49146-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="49146-104">A tartalom keresése/exportálása adatvesztést vagy nem várt adatot ad eredményül.</span><span class="sxs-lookup"><span data-stu-id="49146-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="49146-105">a eDiscovery keresés vagy exportálás nem sikerült</span><span class="sxs-lookup"><span data-stu-id="49146-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="49146-106">Ennek oka az lehet, hogy bizonyos megfelelőségi biztonsági szűrők egy bizonyos rendszergazda által lettek beállítva, és nem lettek közölve az összes rendszergazdával.</span><span class="sxs-lookup"><span data-stu-id="49146-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="49146-107">A probléma megoldásához győződjön meg arról, hogy vannak-e olyan megfelelőségi biztonsági szűrők, amelyek a következő problémákat okozhatják:</span><span class="sxs-lookup"><span data-stu-id="49146-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="49146-108">Csatlakozás a biztonsági és megfelelőségi központ Powershellhez</span><span class="sxs-lookup"><span data-stu-id="49146-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="49146-109">Futtassa az alábbi parancsmaggal található:</span><span class="sxs-lookup"><span data-stu-id="49146-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="49146-110">A megfelelőségi biztonsági szűrőkről további információt a [tartalom keresése engedélyek szűrése](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search) című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="49146-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
