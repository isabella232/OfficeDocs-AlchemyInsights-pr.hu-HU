---
title: A Windows Virtual Desktop szolgáltatás diagnosztikai eszköze
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678622"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="4327a-102">A Windows Virtual Desktop szolgáltatás diagnosztikai eszköze</span><span class="sxs-lookup"><span data-stu-id="4327a-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="4327a-103">A Windows Virtual Desktop (WVD) diagnosztikai eszköz segítségével a rendszergazdák egyetlen felületen azonosíthatják a hibákat.</span><span class="sxs-lookup"><span data-stu-id="4327a-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="4327a-104">Ez az eszköz diagnosztikai információkat naplóz, ha a WVD a WVD szerepkört hozzárendelt valaki használja.</span><span class="sxs-lookup"><span data-stu-id="4327a-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="4327a-105">Az egyes naplók információkat tartalmaznak a tevékenységben részt vevő WVD szerepről, a munkamenet során megjelenő hibaüzenetekről, valamint a bérlőről és a felhasználóról szóló információkról.</span><span class="sxs-lookup"><span data-stu-id="4327a-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="4327a-106">Az Azure log Analytics beállítható úgy, hogy a diagnosztikai eszköz által létrehozott műveletnapló rögzítse a naplót.</span><span class="sxs-lookup"><span data-stu-id="4327a-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="4327a-107">Ezt a következőképpen teheti meg:</span><span class="sxs-lookup"><span data-stu-id="4327a-107">Here's how:</span></span>

1. <span data-ttu-id="4327a-108">Hozzon létre egy log Analytics-munkaterületet az [Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) vagy az [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)segítségével.</span><span class="sxs-lookup"><span data-stu-id="4327a-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="4327a-109">[Windows-számítógépek csatlakoztatása az Azure monitorhoz](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="4327a-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="4327a-110">A munkaterület-azonosító és a munkaterület elsődleges kulcsának beszerzése.</span><span class="sxs-lookup"><span data-stu-id="4327a-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="4327a-111">A beállítási varázslónak szüksége van erre az információra az ügynök megfelelő konfigurálásához és az Azure monitorral való kommunikációhoz.</span><span class="sxs-lookup"><span data-stu-id="4327a-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="4327a-112">[A diagnosztika adatainak leküldése a munkaterületre](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="4327a-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="4327a-113">A diagnosztikai adatait lenyomhatja a WVD-bérlőtől a munkaterülete log-elemzéséhez.</span><span class="sxs-lookup"><span data-stu-id="4327a-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="4327a-114">[Azonosíthatja és diagnosztizálhatja](https://go.microsoft.com/fwlink/?linkid=2128338) az WVD kapcsolatos belső vagy külső problémákat.</span><span class="sxs-lookup"><span data-stu-id="4327a-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="4327a-115">Ha többet szeretne tudni a WVD szolgáltatás diagnosztikai eszközének konfigurálásáról, olvassa el [a naplózási elemzés használata a diagnosztikai szolgáltatáshoz](https://go.microsoft.com/fwlink/?linkid=2128084)című témakört.</span><span class="sxs-lookup"><span data-stu-id="4327a-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
