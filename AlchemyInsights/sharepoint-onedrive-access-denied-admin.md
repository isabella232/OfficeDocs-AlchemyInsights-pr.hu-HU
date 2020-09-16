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
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767664"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Hozzáférés megtagadva üzenetek hibaelhárítása a SharePoint/OneDrive felügyeleti központban

Ha egy SharePoint-vagy OneDrive felügyeleti központra való tallózáskor hozzáférés-megtagadási üzenetet kap, győződjön meg arról, hogy a [felhasználónak licencet kell rendelnie a felhasználóhoz](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Ha a felhasználó rendelkezik licenccel, gondoskodnia kell arról is, hogy a rendszergazdai központokhoz hozzáférő [rendszergazdai szerepkört rendeljen](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) hozzájuk.

Ez a probléma akkor is előfordulhat, ha egy felhasználó törlődik, és újból létrejön ugyanazzal a egyszerű felhasználónévsel (UPN). Az új fiókot egy másik PUID (Passport egyedi azonosító) használatával hozza létre. Amikor a felhasználó megkísérel hozzáférni egy webhelycsoportban vagy a OneDrive, a felhasználó helytelen PUID rendelkezik. A második forgatókönyv a címtár-szinkronizálást jelenti Active Directory-beli szervezeti egységgel (OU). Ha a felhasználók már bejelentkezett a SharePointba, és egy másik szervezeti egységbe vannak áthelyezve, és a SharePointtal újra szinkronizálják őket, előfordulhat, hogy ez a probléma tapasztalható.

A probléma megoldásához vissza kell állítania az eredeti UPN-t a cikkben ismertetett lépésekkel, ha [vissza szeretne állítani egy felhasználót a Microsoft 365-ban](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Megjegyzés: Ha egy OneDrive vagy SharePoint felügyeleti központ nem érhető el több olyan felhasználónál, aki korábban hozzáféréssel rendelkezik, előfordulhat, hogy ideiglenes szolgáltatási probléma van.  [Ellenőrizze a szolgáltatás állapota irányítópultot](https://portal.office.com/adminportal/home#/servicehealth).


