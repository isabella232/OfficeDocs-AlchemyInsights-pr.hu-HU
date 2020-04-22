---
title: A OneDrive Vállalati verzió Web OneDrive átirányítása a Delve-re
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: cbf3db148e16ba6631e9077f893a18d3e1b977af
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722812"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Átirányítva a Delve-re, miután a OneDrive-ra kattintott

Tekintse meg részletes [hibaelhárítási útmutatónkat.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

A probléma megoldásához a rendszergazdának fel kell adnia a felhasználóknak a jogot a Saját helyek webhely ük létrehozására. Ennek az az oka, hogy a OneDrive Vállalati verzió lap a Saját helyek lapon jön létre.

A jog megadásához kövesse az alábbi lépéseket:

1. A SharePoint Felügyeleti központban kattintson a **felhasználói profilok**elemre.

2. A **Kapcsolatok** csoportban kattintson a **Felhasználói engedélyek kezelése gombra.**

3. Adjon hozzá olyan felhasználókat, akiknek engedélyre van szükségük a Saját helyek webhely létrehozásához. Alapértelmezés szerint ez a beállítás a **külső felhasználók kivételével mindenki**értékre van állítva.

4. Miután hozzáadta a felhasználót, felhasználókat vagy csoportot, győződjön meg arról, hogy a hozzáadott felhasználó, felhasználók vagy csoport ki van jelölve, görgessen az **engedélyek** szakaszhoz, majd jelölje be a **Személyes webhely létrehozása (személyes tároláshoz, hírcsatorna és követett tartalomhoz szükséges)** jelölőnégyzetet.

5. Kattintson **az OK gombra,** majd keresse meg a felhasználót a OneDrive-lapon a webhely létrehozásához.
