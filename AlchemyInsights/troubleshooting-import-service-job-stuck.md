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
# <a name="troubleshooting-import-service-job-stuck"></a>Az importálási szolgáltatás elakadt hibáinak elhárítása

Ha problémákat tapasztal a szolgáltatási feladatok importálása vagy sikertelen importálása során, vizsgálja meg a következőt, és próbálkozzon az alábbiakkal:

- Ellenőrizze a PST-fájl méretét. A PST-fájlok maximálisan ajánlott mérete 20 GB.

- Ha azt gyanítja, hogy sérülés miatt kihagyott elemeket kihagyott, futtassa Scanpst.exe a PST-fájlok hibáinak diagnosztizálásához és kijavításához.

- Ha a "MapiExceptionShutoffQuotaExceeded" hibaüzenet jelenik meg az importálás során, győződjön meg arról, hogy a célpostafiók elegendő kapacitással rendelkezik a kívánt PST-fájlok importálására.

A PST-importálási feladatokkal kapcsolatos hibák elhárításáról további információt A PST-importálási feladatokkal kapcsolatos [problémák elhárítása témakörben kaphat.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

A PST-fájloknak a Outlook-be történő importálása során kapcsolatos problémák megoldását A [Outlook .pst fájlok (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)problémáinak elhárítása.