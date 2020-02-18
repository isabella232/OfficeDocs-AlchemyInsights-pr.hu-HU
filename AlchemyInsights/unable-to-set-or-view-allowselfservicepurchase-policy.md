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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091714"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="5e22f-102">Nem lehet beállítani vagy megtekinteni az AllowSelfServicePurchase házirendet</span><span class="sxs-lookup"><span data-stu-id="5e22f-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="5e22f-103">Az AllowSelfServicePurchase házirend beállításakor vagy megtekintésekor a következő hibaüzenet jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="5e22f-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="5e22f-104">*HandleError : Nem sikerült beolvasni a PolicyId "AllowSelfServicePurchase" termékházirendjét, ErrorMessage - Az alapul szolgáló kapcsolat megszakadt: Váratlan hiba történt a küldéssorán.*</span><span class="sxs-lookup"><span data-stu-id="5e22f-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="5e22f-105">Ennek oka lehet a Transport Layer Security (TLS) régebbi verziója.</span><span class="sxs-lookup"><span data-stu-id="5e22f-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="5e22f-106">Az MSCommerce szolgáltatás csatlakoztatásához a TLS 1.2-es vagy nagyobb at kell használnia.</span><span class="sxs-lookup"><span data-stu-id="5e22f-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="5e22f-107">A TLS protokoll 1.2-es engedélyezéséhez/beállításához próbálkozzon az alábbi lépésekkel, ellenőrizze és próbálkozzon újra.</span><span class="sxs-lookup"><span data-stu-id="5e22f-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="5e22f-108">A PowerShell parancssorába (PS C:\) írja be a következő parancsot a TLS protokoll 1.2-es verzióra való beállításához:</span><span class="sxs-lookup"><span data-stu-id="5e22f-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="5e22f-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="5e22f-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="5e22f-110">Ellenőrizze a használatban lévő TLS protokoll(oka)t a következő paranccsal:</span><span class="sxs-lookup"><span data-stu-id="5e22f-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="5e22f-111">\[Net.ServicePointManager]::SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="5e22f-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="5e22f-112">Próbálkozzon újra a Get vagy Update parancsokkal, ha szükséges.</span><span class="sxs-lookup"><span data-stu-id="5e22f-112">Retry the Get or Update commands as needed.</span></span>

