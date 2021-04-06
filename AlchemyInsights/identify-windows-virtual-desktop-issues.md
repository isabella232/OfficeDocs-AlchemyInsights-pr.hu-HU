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
# <a name="identify-windows-virtual-desktop-issues"></a>A Windows virtuális asztal problémáinak azonosítása

A Windows virtuális asztali diagnosztika csak egy PowerShell-parancsmagot használ, de számos opcionális paramétert tartalmaz a problémák szűkítésére és elkülönítésére. Első lépések: 

1. Töltse le és importálja a Windows Virtual Desktop PowerShell modult. Részletes információkért [lásd: Windows Virtuális asztali Windows-parancsmagok a Windows PowerShellhez.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. A fiókjába való bejelentkezéshez futtassa az alábbi parancsmagot:
    
    Példa: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**MEGJEGYZÉS:** A PowerShellt használó összes lekérdezésnek tartalmaznia kell a -UserName vagy -ActivityID paramétert. A figyelőképességről A diagnosztikai funkció naplózási analitikával [( ) nyújt további információ.](https://go.microsoft.com/fwlink/?linkid=2126847)

A diagnosztikai tevékenységek felhasználó szerint való szűréséhez futtassa az alábbi parancsmagot:

Példa: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Megjelenik a problémák diagnosztizálására használható szűrők listája. A problémák diagnosztizálásának további tudnivalókat A Windows virtuális asztali problémáinak azonosítása és [diagnosztizálása.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

A gyakori hibákról a Gyakori hibák – [senarios – cikkből olvashat bővebben.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)
