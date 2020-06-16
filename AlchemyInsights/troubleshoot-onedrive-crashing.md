---
title: A OneDrive összeomlásának elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748921"
---
# <a name="troubleshoot-onedrive-crashes"></a>A OneDrive összeomlásának elhárítása

Ha a OneDrive ismételten összeomlik, próbálkozzon az alábbi hibaelhárítási lépésekkel:

**Győződjön meg arról, hogy a beállításkulcsok nincsenek beállítva:**

1. A Rendszerleíróadatbázis-szerkesztő segítségével keresse meg a HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive mappát
2. Ha a DisableFileSyncNGSC jelen van, és értéke 1, nyissa meg a kulcsot, és módosítsa az értéket 0-ra.
3. A OneDrive manuális elindítása a kezdőképernyőn ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), írja be a OneDrive kifejezést a keresőmezőbe, majd kattintson az asztali OneDrive alkalmazásra.

**OneDrive alaphelyzetbe állítása:**

Megjegyzések:

- A OneDrive alaphelyzetbe állításával leválasztja az összes meglévő szinkronizálási kapcsolatot (beleértve a személyes OneDrive-ot is, ha be van állítva).
- A OneDrive visszaállításával nem veszíti el a fájlokat és az adatokat.

**A OneDrive alaphelyzetbe állítása:**

1. A Futtatás párbeszédpanel megnyitása a Windows billentyű és az R billentyű lenyomásával.
2. Írja be a(z) %localappdata%\Microsoft\OneDrive\onedrive.exe /reset parancsot, és nyomja le az OK gombot. Rövid ideig megjelenhet egy parancsablak.
3. A OneDrive manuális elindítása a kezdőképernyőn ![Nyomja le a Windows billentyűt](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), írja be a OneDrive kifejezést a keresőmezőbe, majd kattintson az asztali OneDrive alkalmazásra.

Megjegyzések:

- Ha úgy döntött, hogy csak néhány mappát szinkronizál az alaphelyzetbe állítás előtt, akkor ezt újra meg kell tennie, miután a szinkronizálás befejeződött. További [információért válassza ki, hogy mely OneDrive-mappákat szeretné szinkronizálni a](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   számítógéppel.
- Ezt személyes OneDrive-ja és OneDrive Vállalati verziója esetén is el kell végeznie.