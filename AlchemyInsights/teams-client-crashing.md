---
title: Összeomlik a Teams ügyfélprogram?
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826273"
---
# <a name="teams-client-crashing"></a>Összeomlik a Teams ügyfélprogram?

Ha összeomlik a Teams ügyfélprogram, próbálkozzon az alábbiakkal:

- Ha a Teams asztali appot használja, [ellenőrizze, hogy az app frissítése teljes-e](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Győződjön meg arról, hogy a [Microsoft 365 összes URL-címe és címtartománya](https://docs.microsoft.com/microsoftteams/connectivity-issues) elérhető.

- Jelentkezzen be a bérlőhöz tartozó rendszergazdai fiókjával, és a [Szolgáltatásállapot irányítópultot](https://docs.microsoft.com/office365/enterprise/view-service-health) ellenőrizve győződjön meg arról, hogy nincs kimaradás vagy teljesítménycsökkenés a szolgáltatás működésében.

- Távolítsa el, majd telepítse újra a Teams alkalmazást (hivatkozás).
    - Tallózással nyissa meg a számítógépen az %appdata%\Microsoft\teams\ mappát, és törölje a benne lévő összes fájlt.
    - [Töltse le és telepítse a Teams alkalmazást](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), és lehetőség szerint rendszergazdaként végezze el a Teams telepítését (kattintson a jobb gombbal a Teams telepítőjére, és válassza a „Futtatás rendszergazdaként” menüpontot, ha elérhető).

Ha a Teams ügyfélprogram továbbra is összeomlik, reprodukálható a probléma? Ha igen:

1. A Problémarögzítő használatával rögzítse az elvégzett lépéseket.
    - Zárja be az ÖSSZES szükségtelen vagy bizalmas alkalmazást.
    - Indítsa el a Problémarögzítőt, és reprodukálja a problémát úgy, hogy közben az érintett felhasználói fiókkal van bejelentkezve.
    - [Gyűjtse össze a rögzített reprodukálási lépéseket tartalmazó Teams-naplókat](https://docs.microsoft.com/microsoftteams/log-files). **Megjegyzés**: Ügyeljen arra, hogy rögzítse az érintett felhasználó bejelentkezési címét.
    - Gyűjtse össze a memóriaképek és/vagy hibagyűjtők adatait (Windows). Indítsa el a Windows PowerShellt azon a gépen, amelyen az összeomlás előfordul, és futtassa az alábbi parancsokat:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Csatolja a fájlt a támogatási esethez.
