---
title: Letöltés letiltása megosztási hivatkozásokon
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358041"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="de42b-102">Letöltés letiltása megosztási hivatkozásokon</span><span class="sxs-lookup"><span data-stu-id="de42b-102">Block download on sharing links</span></span>

<span data-ttu-id="de42b-103">**A blokkletöltés** **csak office-dokumentumokra mutató megtekintési hivatkozásokesetén** érhető el.</span><span class="sxs-lookup"><span data-stu-id="de42b-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="de42b-104">Ha ezt a lehetőséget választja, azok a személyek, akik a létrehozott hivatkozáson keresztül férnek hozzá a fájlhoz, nem látják a fájl letöltési, nyomtatási vagy másolási lehetőségeit.</span><span class="sxs-lookup"><span data-stu-id="de42b-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="de42b-105">A rendszergazdák a `BlockDownloadLinksFileType` [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) vagy a [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell parancsmagok beállításának módosításával szabályozhatják, hogy a "blokkletöltés" beállítás csak office-fájlok esetén jelenjen-e meg.</span><span class="sxs-lookup"><span data-stu-id="de42b-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>