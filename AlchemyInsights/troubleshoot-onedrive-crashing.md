---
title: A OneDrive összeomlásának elhárítása
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826201"
---
# <a name="troubleshoot-onedrive-crashes"></a>A OneDrive összeomlásának elhárítása

Ha a OneDrive ismétlődően összeomlik, próbálkozzon az alábbi hibaelhárítási lépésekkel:

**Győződjön meg arról, hogy nincsenek beállítva beállításkulcsok:**

1. A Beállításszerkesztővel lépjen a HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ha a DisableFileSyncNGSC 1 értékre van állítva, nyissa meg a kulcsot, és módosítsa az értéket 0-ra.
3. Indítsa el manuálisan a OneDrive-ot a Start menüben ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), írja be a OneDrive keresőt a keresőmezőbe, majd kattintson az asztali OneDrive appra.

**A OneDrive alaphelyzetbe állítása:**

Megjegyzések:

- A OneDrive alaphelyzetbe állításával az összes meglévő szinkronizálási kapcsolatot leválasztja (beleértve a személyes OneDrive-ot is, ha be van állítva).
- A OneDrive számítógépen való alaphelyzetbe állításával nem veszít el fájlokat vagy adatokat.

**A OneDrive alaphelyzetbe állítása:**

1. Nyisson meg egy Futtatás párbeszédpanelt a Windows billentyű és az R billentyű lenyomásával.
2. Írja be a %localappdata%\Microsoft\OneDrive\onedrive.exe /reset parancsot, és nyomja le az OK gombot. A parancsablak röviden megjelenhet.
3. Indítsa el manuálisan a OneDrive-ot a Start menüben ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), írja be a OneDrive keresőt a keresőmezőbe, majd kattintson az asztali OneDrive appra.

Megjegyzések:

- Ha úgy döntött, hogy csak bizonyos mappákat szinkronizál az alaphelyzetbe állítás előtt, azt a szinkronizálás befejezése után ismét el kell indítania. További információ: A [számítógépre szinkronizálni kívánt OneDrive-mappák](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   kiválasztása.
- Ezt személyes OneDrive- és OneDrive Vállalati verziós tárterülete esetén kell végrehajtania.