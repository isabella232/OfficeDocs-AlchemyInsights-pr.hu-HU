---
title: A PST-fájlok importálásával kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826165"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="c9aa4-102">A PST-fájlok importálásával kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="c9aa4-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="c9aa4-103">Ha magán az Outlook-ügyfélprogramon belül importál, olvassa el [Az Outlook .pst fájl importálásakor jelentkező problémák elhárítása](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e) című témakört.</span><span class="sxs-lookup"><span data-stu-id="c9aa4-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="c9aa4-104">Ha az importálási szolgáltatás használja, akkor annak elakadása esetén kérjük, vegye figyelembe, hogy az Azure Storage tárhelyre feltöltött egyes PST-fájlok mérete nem lehet nagyobb, mint 20 GB.</span><span class="sxs-lookup"><span data-stu-id="c9aa4-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="c9aa4-105">A 20 GB-nál nagyobb PST-fájlok befolyásolhatják a PST-importálási folyamat teljesítményét.</span><span class="sxs-lookup"><span data-stu-id="c9aa4-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="c9aa4-106">Ha ellenőrizni szeretné egy adott importálási feladat állapotát, használja a következőt: [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="c9aa4-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="c9aa4-107">Az importálási szolgáltatásról további információt [A szervezet PST-fájljainak importálása – áttekintés ](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="c9aa4-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
