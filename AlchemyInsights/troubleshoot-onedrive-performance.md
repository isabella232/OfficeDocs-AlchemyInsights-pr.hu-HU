---
title: A OneDrive teljesítményének elhárítása
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757887"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="68bfc-102">A OneDrive teljesítményének elhárítása</span><span class="sxs-lookup"><span data-stu-id="68bfc-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="68bfc-103">Ha a vártnál lassabb szinkronizálást tapasztal, vagy hasonló teljesítménnyel kapcsolatos problémákat tapasztal a OneDrive:</span><span class="sxs-lookup"><span data-stu-id="68bfc-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="68bfc-104">Ellenőrizze, hogy nincsenek-e ismert problémák a [szolgáltatás állapota irányítópult](https://portal.office.com/adminportal/home?ref=/servicehealth)használatával.</span><span class="sxs-lookup"><span data-stu-id="68bfc-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="68bfc-105">[Szükség esetén engedélyezze a fájlokat](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) a OneDrive-ban, anélkül, hogy le kellene töltenie az összes fájlt, és tárterületet kell használnia az eszközén.</span><span class="sxs-lookup"><span data-stu-id="68bfc-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="68bfc-106">[Tekintse át a gyakorlati tanácsokat](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) a hálózat tervezéséhez és teljesítményéhez.</span><span class="sxs-lookup"><span data-stu-id="68bfc-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="68bfc-107">A [feltöltési és letöltési sebesség maximalizálása](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), különösen akkor, ha az eszközt első alkalommal szinkronizálja.</span><span class="sxs-lookup"><span data-stu-id="68bfc-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="68bfc-108">Ha több mint 100 000-elemmel szinkronizál egy tárat, előfordulhat, hogy a OneDrive szinkronizálása hosszú ideig elakad, vagy az állapot a xMB feldolgozási 0KB jeleníti meg.</span><span class="sxs-lookup"><span data-stu-id="68bfc-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="68bfc-109">További [információ a 100 000-fájlok szinkronizálásáról](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , illetve a [OneDrive által támogatott 300 000-fájlokról](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="68bfc-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="68bfc-110">Ha egy felhasználó túllépi a használati korlátozásokat, a SharePoint Online a felhasználói fióktól érkező további kérelmeket rövid időre szabályozza.</span><span class="sxs-lookup"><span data-stu-id="68bfc-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="68bfc-111">A rendszer minden felhasználó műveletét szabályozza, miközben a fojtószelep van hatályban.</span><span class="sxs-lookup"><span data-stu-id="68bfc-111">All user actions are throttled while the throttle is in effect.</span></span>
