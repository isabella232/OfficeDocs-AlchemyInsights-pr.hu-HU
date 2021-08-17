---
title: Hozzáférés megtagadott üzenetekkel kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085230"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Hozzáférés-megtagadott üzenetek hibaelhárítása a SharePoint/OneDrive Felügyeleti központban

Ha egy SharePoint/OneDrive Felügyeleti központba való tallózáskor hozzáférés-megtagadásról kapott üzenetet, győződjön meg arról, hogy hozzárendelt egy licencet [a felhasználóhoz.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Ha a felhasználónak van licence, akkor [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) azt is meg kell győződni arról, hogy olyan rendszergazdai szerepkört kap, amely hozzáfér a felügyeleti központokhoz.

Ez a probléma akkor is előfordulhat, ha egy felhasználót törölnek és újra létrehoznak ugyanazokkal az egyszerű felhasználónévvel. Az új fiók egy másik PUID (Passport Unique ID) érték használatával jön létre. Amikor a felhasználó megpróbál elérni egy webhelycsoportot vagy a hozzácsat OneDrive, helytelen PUID azonosítót ad meg. A második forgatókönyv a címtár-szinkronizálást is magában foglalja egy Active Directory-szervezeti egységben. Ha a felhasználók már bejelentkeztek a SharePoint, majd egy másik szervezeti egységbe áthelyezik őket, és újraszinkronizációs SharePoint, akkor ez a probléma jelentkezhet.

A probléma megoldásához állítsa vissza az eredeti egyszerű felhasználószámot a Következő cikkben található lépésekkel: Felhasználó [visszaállítása a](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)Microsoft 365.

Megjegyzés: Ha egy OneDrive vagy SharePoint felügyeleti központ nem érhető el több, korábban hozzáféréssel rendelkező felhasználó számára, átmeneti szolgáltatás-probléma lehet.  [Ellenőrizze a szolgáltatás állapot-irányítópultját.](https://portal.office.com/adminportal/home#/servicehealth)


