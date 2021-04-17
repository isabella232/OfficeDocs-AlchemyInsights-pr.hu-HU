---
title: Az Office terminálkiszolgálón történő telepítésével kapcsolatos problémák megoldása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: 447fee84edc65861dc04038cfe6424249e94f843
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823609"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="d3e79-102">Az Office terminálkiszolgálón történő telepítésével kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="d3e79-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="d3e79-103">A megosztott számítógép aktiválásához olyan előfizetéssel kell rendelkezik, amely nagyvállalati Microsoft 365-alkalmazásokat tartalmaz.</span><span class="sxs-lookup"><span data-stu-id="d3e79-103">To use shared computer activation, you must have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>
  
- <span data-ttu-id="d3e79-104">Annak ellenőrzése, hogy engedélyezve van-e a megosztott számítógép aktiválása</span><span class="sxs-lookup"><span data-stu-id="d3e79-104">Verify that shared computer activation is enabled</span></span>
- <span data-ttu-id="d3e79-105">Az aktiválás sikeres voltának ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="d3e79-105">Verify that activation succeeded</span></span>
- <span data-ttu-id="d3e79-106">Tekintse át a megosztott számítógép aktiválására vonatkozó hibaüzeneteket:</span><span class="sxs-lookup"><span data-stu-id="d3e79-106">Review error messages for shared computer activation:</span></span>
- <span data-ttu-id="d3e79-107">"A fiókjában talált termékek nem használhatók az Office aktiválására megosztott számítógépes helyzetekben"</span><span class="sxs-lookup"><span data-stu-id="d3e79-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="d3e79-108">Ez a hiba azt jelzi, hogy nincs olyan előfizetése, amely a Nagyvállalati Microsoft 365-alkalmazásokat tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="d3e79-108">This error means that you don't have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>

<span data-ttu-id="d3e79-109">"Nem licencelt termék"</span><span class="sxs-lookup"><span data-stu-id="d3e79-109">"Unlicensed Product"</span></span>

- <span data-ttu-id="d3e79-110">Ellenőrizze, hogy a felhasználó rendelkezik-e licenccel a Nagyvállalati Microsoft 365-alkalmazásokhoz.</span><span class="sxs-lookup"><span data-stu-id="d3e79-110">Check that the user is assigned a license for Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="d3e79-111">Ellenőrizze, hogy a felhasználó bejelentkezik-e a felhasználói fiókjával.</span><span class="sxs-lookup"><span data-stu-id="d3e79-111">Check that the user signs in with their user account.</span></span>
- <span data-ttu-id="d3e79-112">Ellenőrizze, hogy van-e kapcsolat a megosztott számítógép és az internet között.</span><span class="sxs-lookup"><span data-stu-id="d3e79-112">Check that there is connectivity between the shared computer and the Internet.</span></span>

<span data-ttu-id="d3e79-113">További hibaelhárítási tippeket a következő témakörben talál: [Megosztott számítógép aktiválásával kapcsolatos hibák elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="d3e79-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span></span>