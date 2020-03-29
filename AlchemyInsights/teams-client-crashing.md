---
title: Összeomlik a Teams ügyfélprogram?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030581"
---
# <a name="teams-client-crashing"></a>Összeomlik a Teams ügyfélprogram?

Ha összeomlik a Teams ügyfélprogram, próbálkozzon az alábbiakkal:

- Ha a Teams asztali appot használja, [ellenőrizze, hogy az app frissítése teljes-e](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Győződjön meg arról, hogy az [Office 365 URL-címei és címtartományai](https://docs.microsoft.com/microsoftteams/connectivity-issues) elérhetők.

- Jelentkezzen be a rendszergazdai fiókjával, és a [Szolgáltatásállapot irányítópultot](https://docs.microsoft.com/office365/enterprise/view-service-health) ellenőrizve erősítse meg, hogy nincs kimaradás vagy szolgáltatásiteljesítmény-csökkenés.

 - Utolsó lépésként megpróbálhatja törölni a Teams ügyféloldali gyorsítótárát:

    1.  Lépjen ki teljesen a Microsoft Teams asztali ügyfélprogramból. Kattinthat a jobb gombbal a **Teams** ikonjára az ikontálcán, majd a **Kilépés** parancsra, illetve futtathatja a Feladatkezelőt, és teljesen leállíthatja a folyamatot.

    2.  Nyissa meg a Fájlkezelőt, és írja be a következőt: %appdata%\Microsoft\teams.

    3.  A könyvtárban az alábbi mappák közül látható néhány:

         - Az **alkalmazás-gyorsítótáron** belül nyissa meg a gyorsítótárat, és törölje a fájlok bármelyikét a gyorsítótár helyén: %appdata%\Microsoft\teams\application cache\cache.

        - A **blobtárolóban** törölje az összes fájlt: %appdata%\Microsoft\teams\blob_storage.

        - A **gyorsítótárban** törölje az összes fájlt: %appdata%\Microsoft\teams\Cache.

        - Az **adatbázisokban** törölje az összes fájlt: %appdata%\Microsoft\teams\databases.

        - Az **GPU-gyorsítótárban** törölje az összes fájlt: %appdata%\Microsoft\teams\GPUcache.

        - Az **IndexedDB**, helyen törölje a .db fájlt: %appdata%\Microsoft\teams\IndexedDB.

        - A **helyi tárhelyen** törölje az összes fájlt: %appdata%\Microsoft\teams\Local Storage.

        - Végül a **tmp** könyvtárban törölje bármelyik fájlt: %appdata%\Microsoft\teams\tmp.

    4. Indítsa újra a Teams ügyfélprogramot.
