---
title: OneDrive Vállalati verzió Web OneDrive redirects to Delve
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
ms.openlocfilehash: 295dea987cd14ea848d2bf802f57429642d554b9661dc4dbfc805a447b7d0ede
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922989"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>A hivatkozásra Delve kattintva átirányítja a OneDrive

Tekintse meg részletes [hibaelhárítási útmutatónkat.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

A probléma megoldásához a rendszergazdának meg kell hoznia a felhasználóknak a saját webhelyek létrehozására vonatkozó jogot. Ennek az az oka, OneDrive Vállalati verzió lap a Saját helyek lapon jön létre.

A jog megadásához kövesse az alábbi lépéseket:

1. A felügyeleti SharePoint kattintson a **felhasználói profilok elemre.**

2. A Személyek **csoportban** kattintson a **Felhasználói engedélyek kezelése elemre.**

3. Vegyen fel felhasználókat, akiknek engedélyre van szükségük a Saját helyek webhely létrehozásához. Ez a beállítás alapértelmezés szerint Mindenki, kivéve külső **felhasználók beállításra van állítva.**

4. Miután hozzáadta a felhasználót, felhasználókat vagy csoportot, győződjön meg arról, hogy a hozzáadott  felhasználó, felhasználók vagy csoport ki van jelölve, görgessen az Engedélyek szakaszhoz, és jelölje be a Személyes webhely létrehozása **(személyes tárhelyhez,** hírcsatornához és követett tartalomhoz szükséges) melletti jelölőnégyzetet.

5. Kattintson **az OK** gombra, majd a webhely létrehozásához keresse meg OneDrive lapját.
