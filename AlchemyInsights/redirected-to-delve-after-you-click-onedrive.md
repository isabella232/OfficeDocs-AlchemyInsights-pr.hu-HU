---
title: A OneDrive Vállalati webalkalmazás átirányítja a Delve-et
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799991"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Átirányítva a Delve-be, miután a OneDrive-ra kattintott

Tekintse meg részletes [hibaelhárítási útmutatónkat.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

A probléma megoldásához a rendszergazdának meg kell hoznia a felhasználóknak a saját webhelyek létrehozására vonatkozó jogot. Ennek az az oka, hogy a OneDrive Vállalati verzió lap a Saját helyek lapon jön létre.

A jog megadásához kövesse az alábbi lépéseket:

1. A SharePoint Felügyeleti központban kattintson a **felhasználói profilok elemre.**

2. A Személyek **csoportban** kattintson a **Felhasználói engedélyek kezelése elemre.**

3. Vegyen fel felhasználókat, akiknek engedélyre van szükségük a Saját helyek webhely létrehozásához. Ez a beállítás alapértelmezés szerint Mindenki, kivéve külső **felhasználók beállításra van állítva.**

4. Miután hozzáadta a felhasználót, felhasználókat vagy csoportot, győződjön meg arról, hogy a hozzáadott  felhasználó, felhasználók vagy csoport ki van jelölve, görgessen az Engedélyek szakaszhoz, és jelölje be a Személyes webhely létrehozása **(személyes tárhelyhez,** hírcsatornához és követett tartalomhoz szükséges) melletti jelölőnégyzetet.

5. Kattintson **az OK** gombra, majd a webhely létrehozásához keresse meg a OneDrive lapot.
