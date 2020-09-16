---
title: Nem lehet beállítani vagy megtekinteni a AllowSelfServicePurchase házirendjét
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735201"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="63a2b-102">Nem lehet beállítani vagy megtekinteni a AllowSelfServicePurchase házirendjét</span><span class="sxs-lookup"><span data-stu-id="63a2b-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="63a2b-103">A AllowSelfServicePurchase házirend beállításakor vagy megtekintésekor a következő hibaüzenet jelenik meg:</span><span class="sxs-lookup"><span data-stu-id="63a2b-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="63a2b-104">*HandleError: nem sikerült lekérdezni a termékkulcsot a PolicyId "AllowSelfServicePurchase" ErrorMessage – az alapul szolgáló kapcsolat bezárult: váratlan hiba történt a küldéskor.*</span><span class="sxs-lookup"><span data-stu-id="63a2b-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="63a2b-105">Ennek oka az lehet, hogy a Transport Layer Security (TLS) régebbi verziójával rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="63a2b-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="63a2b-106">A MSCommerce szolgáltatás csatlakoztatásához TLS 1,2 vagy újabbt kell használnia.</span><span class="sxs-lookup"><span data-stu-id="63a2b-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="63a2b-107">A következő lépésekkel engedélyezheti/állíthatja be a TLS-protokollt a 1,2-ra, az ellenőrzésre és az újrapróbálkozásra.</span><span class="sxs-lookup"><span data-stu-id="63a2b-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="63a2b-108">A PowerShell parancssorába (PS C: \) írja be a következő parancsot a 1,2-es verzió TLS-protokolljának beállításához:</span><span class="sxs-lookup"><span data-stu-id="63a2b-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="63a2b-109">Ellenőrizze a használatban lévő TLS protokollt (ka) t, a következő paranccsal:</span><span class="sxs-lookup"><span data-stu-id="63a2b-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="63a2b-110">Szükség esetén próbálkozzon újra a Get vagy a Update parancs segítségével.</span><span class="sxs-lookup"><span data-stu-id="63a2b-110">Retry the Get or Update commands as needed.</span></span>

