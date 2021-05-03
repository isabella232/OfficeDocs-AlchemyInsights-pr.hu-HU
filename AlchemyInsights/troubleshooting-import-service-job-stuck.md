---
title: Az importálási szolgáltatás elakadt hibáinak elhárítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125110"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="f279c-102">Az importálási szolgáltatás elakadt hibáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="f279c-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="f279c-103">Ha problémákat tapasztal a szolgáltatási feladatok importálása vagy sikertelen importálása során, vizsgálja meg a következőt, és próbálkozzon az alábbiakkal:</span><span class="sxs-lookup"><span data-stu-id="f279c-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="f279c-104">Ellenőrizze a PST-fájl méretét.</span><span class="sxs-lookup"><span data-stu-id="f279c-104">Review the size of of the PST file.</span></span> <span data-ttu-id="f279c-105">A PST-fájlok maximálisan ajánlott mérete 20 GB.</span><span class="sxs-lookup"><span data-stu-id="f279c-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="f279c-106">Ha azt gyanítja, hogy sérülés miatt kihagyott elemeket kihagyott, futtassa Scanpst.exe a PST-fájlok hibáinak diagnosztizálásához és kijavításához.</span><span class="sxs-lookup"><span data-stu-id="f279c-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="f279c-107">Ha a "MapiExceptionShutoffQuotaExceeded" hibaüzenet jelenik meg az importálás során, győződjön meg arról, hogy a célpostafiók elegendő kapacitással rendelkezik a kívánt PST-fájlok importálására.</span><span class="sxs-lookup"><span data-stu-id="f279c-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="f279c-108">A PST-importálási feladatokkal kapcsolatos hibák elhárításáról további információt A PST-importálási feladatokkal kapcsolatos [problémák elhárítása témakörben kaphat.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="f279c-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="f279c-109">A PST-fájloknak a Outlook-be történő importálása során kapcsolatos problémák megoldását A [Outlook .pst fájlok (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)problémáinak elhárítása.</span><span class="sxs-lookup"><span data-stu-id="f279c-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>