---
title: A OneDrive vállalati verzió webes OneDrive átirányítja a ásni-ra
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776381"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Átirányítva ás a OneDrive kattintás után

Részletes [hibaelhárítási útmutatót](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)talál.

A probléma megoldásához a rendszergazdának meg kell adnia a megfelelő jogosultságot a saját webhelyek webhely létrehozásához. Ennek az az oka, hogy a OneDrive vállalati verzió lap jön létre a saját webhelyeken.

A jogosultság megadásához kövesse az alábbi lépéseket:

1. A SharePoint felügyeleti központban kattintson a **felhasználói profilok**elemre.

2. A **személyek** csoportban kattintson a **felhasználói engedélyek kezelése**elemre.

3. Adjon hozzá olyan felhasználókat, akiknek engedélyt kell adni a saját webhelyek webhelyének létrehozásához. Alapértelmezés szerint ez a beállítás a **külső felhasználók kivételével mindenki számára**beállításra van állítva.

4. Miután hozzáadta a felhasználót, felhasználókat vagy csoportot, győződjön meg arról, hogy a hozzáadott felhasználó, felhasználók vagy csoport van kijelölve, és jelölje be az **engedélyek** szakasz jelölőnégyzetét, és jelölje be a **személyes webhely létrehozása (a személyes tárterület, a hírcsatorna és a követett tartalom esetében szükséges)** jelölőnégyzetet.

5. Kattintson az **OK gombra**, majd a felhasználó tallózással keresse meg a OneDrive lapot a webhely létrehozásához.
