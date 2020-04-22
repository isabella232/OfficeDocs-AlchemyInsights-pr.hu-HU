---
title: A OneDrive teljesítményének hibáinak elhárítása
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 197a84c5f69f9e58460925049345263743fe78ee
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43733200"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="a670f-102">A OneDrive teljesítményének hibáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="a670f-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="a670f-103">Ha a vártnál lassabb szinkronizálást vagy hasonló teljesítményproblémákat tapasztal a OneDrive-val:</span><span class="sxs-lookup"><span data-stu-id="a670f-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="a670f-104">Ellenőrizze, hogy nincsenek-e ismert problémák a [Service Health Dashboard használatával.](https://portal.office.com/adminportal/home?ref=/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="a670f-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="a670f-105">[Engedélyezze az igény szerinti fájlokat,](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) hogy az összes fájlt elérhesse a OneDrive-on anélkül, hogy le kellene töltenie az összeset, és tárhelyet kellene használnia az eszközön.</span><span class="sxs-lookup"><span data-stu-id="a670f-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="a670f-106">Tekintse át a hálózattervezéssel és a [teljesítménnyel kapcsolatos gyakorlati tanácsokat.](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance)</span><span class="sxs-lookup"><span data-stu-id="a670f-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="a670f-107">[Maximalizálja a feltöltési és letöltési sebességet,](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)különösen akkor, ha először szinkronizál egy eszközt.</span><span class="sxs-lookup"><span data-stu-id="a670f-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="a670f-108">Ha több mint 100 000 elemet tartalmazó tárat szinkronizál, előfordulhat, hogy a OneDrive-szinkronizálás hosszú ideig beragadt, vagy az állapot a 0 KB xMB feldolgozása látható."</span><span class="sxs-lookup"><span data-stu-id="a670f-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="a670f-109">[További információ a több mint 100 000 fájl szinkronizálásáról,](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) valamint a [OneDrive 300 000-es korlátjáról.](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)</span><span class="sxs-lookup"><span data-stu-id="a670f-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="a670f-110">Ha egy felhasználó túllépi a használati korlátokat, a SharePoint Online rövid időre szabályozza az adott felhasználói fiókból érkező további kérelmeket.</span><span class="sxs-lookup"><span data-stu-id="a670f-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="a670f-111">Minden felhasználói művelet szabályozása, amíg a fojtószelep érvényben van.</span><span class="sxs-lookup"><span data-stu-id="a670f-111">All user actions are throttled while the throttle is in effect.</span></span>
