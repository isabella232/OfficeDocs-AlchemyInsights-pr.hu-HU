---
title: Teams ügyfél összeomlik
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
ms.openlocfilehash: bef16351b55ac4765539d66ab86a71183f66f0dd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321627"
---
# <a name="teams-client-crashing"></a>Teams ügyfél összeomlik

Ha összeomlik a Teams ügyfélprogram, próbálkozzon az alábbiakkal:

- Ha a Teams asztali appot használja, [ellenőrizze, hogy az app frissítése teljes-e](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Győződjön meg arról, hogy a [Microsoft 365 összes URL-címe és címtartománya](https://docs.microsoft.com/microsoftteams/connectivity-issues) elérhető.

- Jelentkezzen be a bérlőhöz tartozó rendszergazdai fiókjával, és a [Szolgáltatásállapot irányítópultot](https://docs.microsoft.com/office365/enterprise/view-service-health) ellenőrizve győződjön meg arról, hogy nincs kimaradás vagy teljesítménycsökkenés a szolgáltatás működésében.

- A telepített alkalmazás Teams újratelepítése
    - Tallózással keresse meg a számítógépen az %appdata%\Microsoft\Teams\ mappát, és törölje a könyvtárban lévő összes fájlt.
    - [Töltse le és telepítse](https://www.microsoft.com/microsoft-teams/download-app)az Teams appot , és ha lehetséges, telepítse az Teams alkalmazást rendszergazdaként  (kattintson a jobb gombbal az Teams telepítőjére, és válassza a Futtatás rendszergazdaként lehetőséget, ha elérhető).

Ha a Teams továbbra is összeomlik, próbálja meg reprodukálni a problémát. Ha van rá szükség:

1. A Problémarögzítő használatával rögzítse az elvégzett lépéseket.
    - Zárja be az ÖSSZES szükségtelen vagy bizalmas alkalmazást.
    - Indítsa el a Problémarögzítőt, és reprodukálja a problémát úgy, hogy közben az érintett felhasználói fiókkal van bejelentkezve.
    - [Gyűjtse össze a rögzített reprodukálási lépéseket tartalmazó Teams-naplókat](https://docs.microsoft.com/microsoftteams/log-files). 
    
    **Megjegyzés**: Ügyeljen arra, hogy rögzítse az érintett felhasználó bejelentkezési címét.
    - Gyűjtse össze a memóriaképek és/vagy hibagyűjtők adatait (Windows). Indítsa Windows Powershellt a gépen, ahol az összeomlás történik, és futtassa az alábbi parancsokat (az egyes parancsok után nyomja le az Enter billentyűt):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Miután létrehozott egy szövegfájlt, és megjelent a képernyőn, mentse a fájlt, és csatolja a szolgáltatáskéréshez. 
