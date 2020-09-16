---
title: Az Office terminálkiszolgálón való telepítésekor felmerülő problémák megoldása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: df1a50031196fbd79662cee620fc41c7be14e179
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738459"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="24637-102">Az Office terminálkiszolgálón való telepítésekor felmerülő problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="24637-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="24637-103">A megosztott számítógép-aktiválás használatához olyan előfizetéssel kell rendelkeznie, amely magában foglalja a Microsoft 365-alkalmazásokat a nagyvállalatoknak.</span><span class="sxs-lookup"><span data-stu-id="24637-103">To use shared computer activation, you must have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>
  
- <span data-ttu-id="24637-104">Annak ellenőrzése, hogy engedélyezve van-e a megosztott számítógép aktiválása</span><span class="sxs-lookup"><span data-stu-id="24637-104">Verify that shared computer activation is enabled</span></span>
- <span data-ttu-id="24637-105">Az aktiválás sikerességének ellenőrzése</span><span class="sxs-lookup"><span data-stu-id="24637-105">Verify that activation succeeded</span></span>
- <span data-ttu-id="24637-106">A megosztott számítógép aktiválásával kapcsolatos hibaüzenetek áttekintése:</span><span class="sxs-lookup"><span data-stu-id="24637-106">Review error messages for shared computer activation:</span></span>
- <span data-ttu-id="24637-107">"A fiókjában talált termékek nem használhatók az Office aktiválásához megosztott számítógépeken"</span><span class="sxs-lookup"><span data-stu-id="24637-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="24637-108">Ez a hibaüzenet azt jelzi, hogy nincs olyan előfizetése, amely tartalmazza a Microsoft 365-alkalmazásokat a nagyvállalatoknak.</span><span class="sxs-lookup"><span data-stu-id="24637-108">This error means that you don't have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>

<span data-ttu-id="24637-109">"Nem licencelt termék"</span><span class="sxs-lookup"><span data-stu-id="24637-109">"Unlicensed Product"</span></span>

- <span data-ttu-id="24637-110">Ellenőrizze, hogy a felhasználóhoz van-e hozzárendelve licenc a Microsoft 365-alkalmazások nagyvállalati verzióhoz.</span><span class="sxs-lookup"><span data-stu-id="24637-110">Check that the user is assigned a license for Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="24637-111">Ellenőrizze, hogy a felhasználó bejelentkezik-e a felhasználói fiókjával.</span><span class="sxs-lookup"><span data-stu-id="24637-111">Check that the user signs in with their user account.</span></span>
- <span data-ttu-id="24637-112">Ellenőrizze, hogy van-e kapcsolat a megosztott számítógép és az internet között.</span><span class="sxs-lookup"><span data-stu-id="24637-112">Check that there is connectivity between the shared computer and the Internet.</span></span>

<span data-ttu-id="24637-113">További hibaelhárítási tippekért lásd: [a megosztott számítógép aktiválásával kapcsolatos problémák elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="24637-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span></span>