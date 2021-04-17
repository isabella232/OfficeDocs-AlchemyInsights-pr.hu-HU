---
title: Nem lehet beállítani vagy megtekinteni az AllowSelfServicePurchase házirendet
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826093"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="73d12-102">Nem lehet beállítani vagy megtekinteni az AllowSelfServicePurchase házirendet</span><span class="sxs-lookup"><span data-stu-id="73d12-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="73d12-103">Az AllowSelfServicePurchase házirend beállításakor vagy megtekintésekor a következő hibaüzenet jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="73d12-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="73d12-104">*HandleError: Nem sikerült beolvasni a termék házirendet a PolicyId 'AllowSelfServicePurchase', ErrorMessage - A mögöttes kapcsolat lezárult: Váratlan hiba történt egy küldéskor.*</span><span class="sxs-lookup"><span data-stu-id="73d12-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="73d12-105">Ezt a Transport Layer Security (TLS) egy régebbi verziója okozhatja.</span><span class="sxs-lookup"><span data-stu-id="73d12-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="73d12-106">Az MSCommerce szolgáltatás csatlakoztatásának 1.2-es vagy újabb TLS-et kell használnia.</span><span class="sxs-lookup"><span data-stu-id="73d12-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="73d12-107">Az alábbi lépésekkel engedélyezze vagy állítsa a TLS protokollt 1.2-esre, ellenőrizze és próbálkozzon újra.</span><span class="sxs-lookup"><span data-stu-id="73d12-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="73d12-108">A PowerShell parancssorában (PS C: a következő paranccsal állítsa a \) TLS protokollt az 1.2-es verzióra:</span><span class="sxs-lookup"><span data-stu-id="73d12-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="73d12-109">Ellenőrizze a használatban van TLS protokollokat az alábbi paranccsal:</span><span class="sxs-lookup"><span data-stu-id="73d12-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="73d12-110">Szükség szerint próbálja meg újból a Get vagy a Update parancsot.</span><span class="sxs-lookup"><span data-stu-id="73d12-110">Retry the Get or Update commands as needed.</span></span>

