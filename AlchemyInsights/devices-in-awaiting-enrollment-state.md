---
title: Regisztrációra váró eszközök
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
- "9000657"
- "2508"
ms.openlocfilehash: 220da7807f178a9dff4a78c61dd3e0cc8004c9c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815356"
---
# <a name="devices-are-in-awaiting-enrollment-state"></a><span data-ttu-id="c4e3b-102">Az eszközök "Regisztrációra vár" állapotban vannak</span><span class="sxs-lookup"><span data-stu-id="c4e3b-102">Devices are in "Awaiting Enrollment" state</span></span>

<span data-ttu-id="c4e3b-103">Az asztali elemzések nem tartalmaznak diagnosztikai adatokat ehhez az eszközhöz.</span><span class="sxs-lookup"><span data-stu-id="c4e3b-103">Desktop Analytics doesn't have diagnostic data for this device.</span></span> 

<span data-ttu-id="c4e3b-104">Ez a probléma azért fordulhat elő, mert nemrégiben hozzáadta az eszközt a célcsoporthoz, és még nem küldött adatokat.</span><span class="sxs-lookup"><span data-stu-id="c4e3b-104">This issue may occur because you recently added the device to the target collection and it hasn't yet sent data.</span></span> <span data-ttu-id="c4e3b-105">Ez azt is jelentheti, hogy az eszköz nem kommunikál megfelelően a szolgáltatással, és a legújabb diagnosztikai adatok több mint 28 naposak.</span><span class="sxs-lookup"><span data-stu-id="c4e3b-105">It can also mean the device isn't properly communicating with the service, and the latest diagnostic data is more than 28 days old.</span></span>

<span data-ttu-id="c4e3b-106">Győződjön meg arról, hogy az eszköz képes kommunikálni a szolgáltatással.</span><span class="sxs-lookup"><span data-stu-id="c4e3b-106">Make sure the device can communicate with the service.</span></span> <span data-ttu-id="c4e3b-107">További információt a [Végpontok .](https://docs.microsoft.com/configmgr/desktop-analytics/enable-data-sharing#endpoints)</span><span class="sxs-lookup"><span data-stu-id="c4e3b-107">For more information, see [Endpoints](https://docs.microsoft.com/configmgr/desktop-analytics/enable-data-sharing#endpoints).</span></span>

<span data-ttu-id="c4e3b-108">A regisztráció állapotát a Kapcsolatállapot figyelése oldalon [láthatja.](https://docs.microsoft.com/configmgr/desktop-analytics/monitor-connection-health#awaiting-enrollment)</span><span class="sxs-lookup"><span data-stu-id="c4e3b-108">For more information about the awaiting enrollment status, see [Monitor Connection Health](https://docs.microsoft.com/configmgr/desktop-analytics/monitor-connection-health#awaiting-enrollment).</span></span>