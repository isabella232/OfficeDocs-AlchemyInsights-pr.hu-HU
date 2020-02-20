---
title: Nem lehet beállítani vagy megtekinteni az AllowSelfServicePurchase házirendet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158563"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="603f4-102">Nem lehet beállítani vagy megtekinteni az AllowSelfServicePurchase házirendet</span><span class="sxs-lookup"><span data-stu-id="603f4-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="603f4-103">Az AllowSelfServicePurchase házirend beállításakor vagy megtekintésekor a következő hibaüzenet jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="603f4-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="603f4-104">*HandleError : Nem sikerült beolvasni a PolicyId "AllowSelfServicePurchase" termékházirendjét, ErrorMessage - Az alapul szolgáló kapcsolat megszakadt: Váratlan hiba történt a küldéssorán.*</span><span class="sxs-lookup"><span data-stu-id="603f4-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="603f4-105">Ennek oka lehet a Transport Layer Security (TLS) régebbi verziója.</span><span class="sxs-lookup"><span data-stu-id="603f4-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="603f4-106">Az MSCommerce szolgáltatás csatlakoztatásához a TLS 1.2-es vagy nagyobb at kell használnia.</span><span class="sxs-lookup"><span data-stu-id="603f4-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="603f4-107">A TLS protokoll 1.2-es engedélyezéséhez/beállításához próbálkozzon az alábbi lépésekkel, ellenőrizze és próbálkozzon újra.</span><span class="sxs-lookup"><span data-stu-id="603f4-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="603f4-108">A PowerShell parancssorába (PS C:\) írja be a következő parancsot a TLS protokoll 1.2-es verzióra való beállításához:</span><span class="sxs-lookup"><span data-stu-id="603f4-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="603f4-109">Ellenőrizze a használatban lévő TLS protokoll(oka)t a következő paranccsal:</span><span class="sxs-lookup"><span data-stu-id="603f4-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="603f4-110">Próbálkozzon újra a Get vagy Update parancsokkal, ha szükséges.</span><span class="sxs-lookup"><span data-stu-id="603f4-110">Retry the Get or Update commands as needed.</span></span>

