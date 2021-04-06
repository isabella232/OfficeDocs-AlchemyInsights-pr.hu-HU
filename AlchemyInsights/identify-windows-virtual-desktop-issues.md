---
title: A Windows virtuális asztal problémáinak azonosítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595850"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="dbf49-102">A Windows virtuális asztal problémáinak azonosítása</span><span class="sxs-lookup"><span data-stu-id="dbf49-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="dbf49-103">A Windows virtuális asztali diagnosztika csak egy PowerShell-parancsmagot használ, de számos opcionális paramétert tartalmaz a problémák szűkítésére és elkülönítésére.</span><span class="sxs-lookup"><span data-stu-id="dbf49-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="dbf49-104">Első lépések:</span><span class="sxs-lookup"><span data-stu-id="dbf49-104">To get started:</span></span> 

1. <span data-ttu-id="dbf49-105">Töltse le és importálja a Windows Virtual Desktop PowerShell modult.</span><span class="sxs-lookup"><span data-stu-id="dbf49-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="dbf49-106">Részletes információkért [lásd: Windows Virtuális asztali Windows-parancsmagok a Windows PowerShellhez.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="dbf49-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="dbf49-107">A fiókjába való bejelentkezéshez futtassa az alábbi parancsmagot:</span><span class="sxs-lookup"><span data-stu-id="dbf49-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="dbf49-108">Példa: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="dbf49-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="dbf49-109">**MEGJEGYZÉS:** A PowerShellt használó összes lekérdezésnek tartalmaznia kell a -UserName vagy -ActivityID paramétert.</span><span class="sxs-lookup"><span data-stu-id="dbf49-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="dbf49-110">A figyelőképességről A diagnosztikai funkció naplózási analitikával [( ) nyújt további információ.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="dbf49-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="dbf49-111">A diagnosztikai tevékenységek felhasználó szerint való szűréséhez futtassa az alábbi parancsmagot:</span><span class="sxs-lookup"><span data-stu-id="dbf49-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="dbf49-112">Példa: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="dbf49-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="dbf49-113">Megjelenik a problémák diagnosztizálására használható szűrők listája.</span><span class="sxs-lookup"><span data-stu-id="dbf49-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="dbf49-114">A problémák diagnosztizálásának további tudnivalókat A Windows virtuális asztali problémáinak azonosítása és [diagnosztizálása.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="dbf49-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="dbf49-115">A gyakori hibákról a Gyakori hibák – [senarios – cikkből olvashat bővebben.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)</span><span class="sxs-lookup"><span data-stu-id="dbf49-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
