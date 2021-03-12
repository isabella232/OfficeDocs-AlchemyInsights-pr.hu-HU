---
title: Hozzáférés megtagadva üzenetek hibaelhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707956"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Hozzáférés megtagadva üzenetek hibaelhárítása a SharePointban és a OneDrive Felügyeleti központban

Ha egy Hozzáférés megtagadva üzenet jelenik meg, amikor egy SharePoint/OneDrive Felügyeleti központot próbál meg böngészni, győződjön meg arról, hogy hozzárendelt egy licencet [a felhasználóhoz.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Ha a felhasználó rendelkezik licenccel, akkor azt is meg kell győződni arról, hogy olyan rendszergazdai szerepkört kap, amely hozzáférhet [a](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) felügyeleti központokhoz.

Ez a probléma akkor is előfordulhat, ha egy felhasználót törölnek, majd újra létrehoznak ugyanazokkal az egyszerű felhasználónévvel. Az új fiók egy másik PUID (Passport Unique ID) értékkel jön létre. Amikor a felhasználó megpróbál hozzáférni egy webhelycsoporthoz vagy a OneDrive-jukhoz, helytelen PUID azonosítót adott meg. A második forgatókönyv az Active Directory szervezeti egységekkel való címtár-szinkronizálást foglalja magában. Ha a felhasználók már bejelentkeztek a SharePointba, majd áthelyezik őket egy másik szervezeti webhelyre, és újraszinkron módon szinkronizálják őket a SharePointtal, akkor előfordulhat, hogy ez a probléma jelentkezik.

A probléma megoldásához állítsa vissza az eredeti egyszerű felhasználószámot a Felhasználó visszaállítása [a Microsoft 365-ben](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)a cikkben található lépésekkel.

Megjegyzés: Ha a OneDrive vagy a SharePoint Felügyeleti központ nem érhető el több, korábban hozzáféréssel rendelkező felhasználónak, átmeneti szolgáltatásbeli probléma lehet.  [Ellenőrizze a szolgáltatás állapot-irányítópultját.](https://portal.office.com/adminportal/home#/servicehealth)


