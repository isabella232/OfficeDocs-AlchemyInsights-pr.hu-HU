---
title: Összeomlást okozó hibák elhárítása OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665000"
---
# <a name="troubleshoot-onedrive-crashes"></a>Összeomlást okozó hibák elhárítása OneDrive

Ha a OneDrive ismétlődően összeomlik, próbálkozzon az alábbi hibaelhárítási lépésekkel:

**Győződjön meg arról, hogy a rendszerleíró kulcsok nem állíthatók be:**

1. A Rendszerleíróadatbázis-szerkesztő segítségével keresse meg a HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Ha a DisableFileSyncNGSC be van állítva, és a 1 értéket adja meg, nyissa meg a kulcsot, és módosítsa az értéket 0-ra.
3. A OneDrive manuális elindítása a Start menüben ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)mezőbe írja be a OneDrive kifejezést, és kattintson az asztali OneDrive alkalmazásra.

**A OneDrive alaphelyzetbe állítása:**

Megjegyzi

- A OneDrive alaphelyzetbe állításával az összes meglévő szinkronizálási kapcsolatot leválasztja (a beállítás esetén a személyes OneDrive is).
- A számítógépén a OneDrive alaphelyzetbe állításával nem veszíthet el fájlokat vagy adatot.

**A OneDrive alaphelyzetbe állítása:**

1. Nyisson meg egy Futtatás párbeszédpanelt a Windows billentyű és az R billentyű lenyomásával.
2. Írja be a% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset, és nyomja le az OK gombot. Előfordulhat, hogy egy parancssorablak is megjelenik röviden.
3. A OneDrive manuális elindítása a Start menüben ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)mezőbe írja be a OneDrive kifejezést, és kattintson az asztali OneDrive alkalmazásra.

Megjegyzi

- Ha úgy döntött, hogy az Alaphelyzetbe állítás előtt csak bizonyos mappákat szinkronizál, akkor a szinkronizálás befejeződése után ismét el kell végeznie ezt a műveletet. További információért olvassa el a [számítógépen szinkronizálandó OneDrive-mappák kiválasztása](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)című témakört   .
- A személyes OneDrive és a OneDrive vállalati verzióhoz ezt el kell végeznie.