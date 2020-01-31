---
title: A OneDrive Vállalati web onedrive átirányítja a Delve-re
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
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571209"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Átirányítva a Delve-re, miután a OneDrive-ra kattintott

Tekintse meg részletes [hibaelhárítási útmutatónkat.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

A probléma megoldásához az Office 365 rendszergazdájának meg kell adnia a felhasználóknak a Saját helyek webhely létrehozásának jogát. Ennek az az oka, hogy a OneDrive Vállalati verzió lap a Saját webhelyek lapon jön létre.

A jog megadásához kövesse az alábbi lépéseket:

1. A SharePoint Felügyeleti központban kattintson a **felhasználói profilok**elemre.

2. A **Kapcsolatok** csoportban kattintson a **Felhasználói engedélyek kezelése**gombra.

3. Adjon hozzá olyan felhasználókat, akiknek engedélyre van szükségük a Saját helyek webhely létrehozásához. Alapértelmezés szerint ez a beállítás **a külső felhasználók kivételével mindenki**re van állítva.

4. Miután felvette a felhasználót, a felhasználókat vagy a csoportot, győződjön meg arról, hogy a hozzáadott felhasználó, felhasználók vagy csoportok be van jelölve, görgessen az **engedélyek** szakaszhoz, majd jelölje be a **Személyes webhely létrehozása (személyes tároláshoz, hírcsatorna és követett tartalomhoz szükséges)** jelölőnégyzetet.

5. Kattintson az **OK**gombra, majd a webhely létrehozásához keresse meg a felhasználót a OneDrive lapon.
