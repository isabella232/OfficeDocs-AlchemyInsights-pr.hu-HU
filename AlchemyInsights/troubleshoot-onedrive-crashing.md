---
title: Összeomlás OneDrive elhárítása
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
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921009"
---
# <a name="troubleshoot-onedrive-crashes"></a>Összeomlás OneDrive elhárítása

Ha OneDrive rendszeresen összeomlik, próbálkozzon az alábbi hibaelhárítási lépésekkel:

**Győződjön meg arról, hogy nincsenek beállítva beállításkulcsok:**

1. A Beállításszerkesztővel lépjen a HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ha a DisableFileSyncNGSC 1 értékre van állítva, nyissa meg a kulcsot, és módosítsa az értéket 0-ra.
3. Indítsa el OneDrive start menüt a Start ![Nyomja le Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), írja OneDrive a keresőmezőbe, majd kattintson a OneDrive alkalmazásra.

**A OneDrive alaphelyzetbe állítása:**

Megjegyzések:

- A OneDrive kapcsolat bontása az összes meglévő szinkronizálási kapcsolatot (beleértve a személyes OneDrive, ha be van állítva).
- Ha a számítógépen alaphelyzetbe OneDrive a fájlokat vagy az adatokat, nem veszíti el a fájlokat és az adatokat.

**A következő OneDrive:**

1. A Futtatás párbeszédpanel megnyitásához nyomja le a Windows és az R billentyűt.
2. Írja be a %localappdata%\Microsoft\OneDrive\onedrive.exe /reset parancsot, és nyomja le az OK gombot. A parancsablak röviden megjelenhet.
3. Indítsa el OneDrive start menüt a Start ![Nyomja le Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), írja OneDrive a keresőmezőbe, majd kattintson a OneDrive alkalmazásra.

Megjegyzések:

- Ha úgy döntött, hogy csak bizonyos mappákat szinkronizál az alaphelyzetbe állítás előtt, azt a szinkronizálás befejezése után ismét el kell indítania. További [információért olvassa el OneDrive, hogy mely mappákat szinkronizálja](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)a   számítógépre.
- Ezt a személyes és a személyes OneDrive kell OneDrive Vállalati verzió.