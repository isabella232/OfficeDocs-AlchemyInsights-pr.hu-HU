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
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354054"
---
# <a name="teams-client-crashing"></a>Összeomlik a Teams ügyfélprogram?

Ha összeomlik a Teams ügyfélprogram, próbálkozzon az alábbiakkal:

- Ha a Teams asztali appot használja, [ellenőrizze, hogy az app frissítése teljes-e](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Győződjön meg arról, hogy a [Microsoft 365 összes URL-címe és címtartománya](https://docs.microsoft.com/microsoftteams/connectivity-issues) elérhető.

- Jelentkezzen be a bérlői rendszergazdai fiókkal, és ellenőrizze a [Szolgáltatásállapot-irányítópultot,](https://docs.microsoft.com/office365/enterprise/view-service-health) és ellenőrizze, hogy nincs-e kimaradás vagy szolgáltatáslebontás.

- A Teams alkalmazás eltávolítása és újratelepítése (hivatkozás)
    - Tallózással keresse meg a számítógép %appdata%\Microsoft\teams\ mappáját, és törölje a könyvtár összes fájlját.
    - [Töltse le és telepítse a Teams alkalmazást,](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)és ha lehetséges, telepítse a Teamst rendszergazdaként (kattintson a jobb gombbal a Teams telepítőjére, és ha elérhető, válassza a "Futtatás rendszergazdaként" lehetőséget).

Ha a Teams-ügyfél még mindig összeomlik, reprodukálhatja a problémát? Ha igen:

1. A lépésrögzítő vel rögzítheti a lépéseket.
    - Zárja be az összes felesleges vagy bizalmas alkalmazást.
    - Indítsa el a Lépésrögzítőt, és reprodukálja a problémát, miközben bejelentkezik az érintett felhasználói fiókkal.
    - [Gyűjtse össze a csapatok naplókat, hogy rögzítse a rögzített repro lépéseket](https://docs.microsoft.com/microsoftteams/log-files). **Megjegyzés:** Győződjön meg arról, hogy rögzíti az érintett felhasználó bejelentkezési címét.
    - Gyűjtse össze a memóriakép és/vagy a Hibagyűjtő adatait (Windows). Indítsa el a Windows Powershell t azon a számítógépen, amelyen az összeomlás történik, és futtassa a következő parancsokat:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Csatolja a fájlt a támogatási esethez.
