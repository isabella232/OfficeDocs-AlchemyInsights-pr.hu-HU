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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059817"
---
# <a name="troubleshooting-pst-import-issues"></a>A PST-fájlok importálásával kapcsolatos hibák elhárítása

- Ha magában az Outlook ügyfélprogramban importál, az Outlook .pst fájl importálása során problémáinak megoldása című [témakörben további témakört is láthat.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Ha importálási szolgáltatást használ, és az elakad, vegye figyelembe, hogy az Azure-tárhelyre feltöltött PST-fájlok mérete nem lehet nagyobb 20 GB-nál. A 20 GB-nál nagyobb PST-fájlok hatással lehetnek a PST-importálási folyamat teljesítményére. A beragadt állások hibaelhárításáról további információt A PST-importálási feladatokat [érintő problémák.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Ha egy adott importálási feladat állapotát szeretné ellenőrizni, használja a [Get-MailboxImportRequest -batchname lehetőséget.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- Az importálási szolgáltatásról további információt A szervezet PST-fájljainak importálása – áttekintés [témakörben talál.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
