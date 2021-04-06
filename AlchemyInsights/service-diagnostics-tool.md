---
title: Service diagnostics tool for Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595869"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="74936-102">Service diagnostics tool for Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="74936-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="74936-103">A Windows Virtual Desktop (WVD) diagnosztikai eszközével a rendszergazdák egyetlen felületen azonosíthatja a hibákat.</span><span class="sxs-lookup"><span data-stu-id="74936-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="74936-104">Ez az eszköz diagnosztikai adatokat naplóz minden alkalommal, amikor egy WVD-szerepkörrel társított felhasználó használja a WVD-et.</span><span class="sxs-lookup"><span data-stu-id="74936-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="74936-105">Minden napló tartalmazza a tevékenységben érintett WVD szerepkört, a munkamenet során megjelenő hibaüzeneteket, valamint a bérlő és a felhasználó adatait.</span><span class="sxs-lookup"><span data-stu-id="74936-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="74936-106">Az Azure Log Analytics konfigurálható a diagnosztikai eszköz által létrehozott tevékenységnapló rögzítésére az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="74936-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="74936-107">Hozzon létre egy Log Analytics munkaterületet az [Azure Portal vagy](https://go.microsoft.com/fwlink/?linkid=2129500) az Azure [PowerShell segítségével.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="74936-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="74936-108">[Windows rendszerű számítógépek csatlakoztatása az Azure Monitorhoz.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="74936-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="74936-109">Szerezze be a munkaterület azonosítóját és a munkaterület elsődleges kulcsát.</span><span class="sxs-lookup"><span data-stu-id="74936-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="74936-110">A beállítási varázslónak szüksége van erre az információra, hogy megfelelően konfigurálja az ügynököt, és biztosítsa, hogy képes legyen kommunikálni az Azure Monitorral.</span><span class="sxs-lookup"><span data-stu-id="74936-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="74936-111">[Leküldéses diagnosztikai adatok a munkaterületre.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="74936-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="74936-112">Leküldéses diagnosztikai adatokat a WVD-bérlőről a munkaterület naplóelemzésébe.</span><span class="sxs-lookup"><span data-stu-id="74936-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="74936-113">[A](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) WVD-vel kapcsolatos belső vagy külső problémák azonosítása és diagnosztizálása.</span><span class="sxs-lookup"><span data-stu-id="74936-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="74936-114">A szolgáltatásdiagnosztikai eszköz WVD-hez való konfigurálásával kapcsolatos további információkért lásd: A diagnosztikai funkció használata a naplóelemzéssel.</span><span class="sxs-lookup"><span data-stu-id="74936-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>