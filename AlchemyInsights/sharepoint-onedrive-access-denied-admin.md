---
title: Hozzáférés megtagadott üzenetek hibáinak elhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505381"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Hozzáférés megtagadott üzenetek hibái a Sharepoint/OneDrive Felügyeleti központban

Ha a Sharepoint/OneDrive Felügyeleti központ megtallásához megkísérelt hozzáférési üzenetet kap, győződjön meg arról, hogy [licencet rendelt a felhasználóhoz.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Ha a felhasználó rendelkezik licenccel, győződjön meg arról is, hogy [rendszergazdai szerepkört kapnak,](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) amely hozzáférhet a felügyeleti központokhoz.

Ez a probléma akkor is előfordulhat, ha egy felhasználót törölnek, és újra létrehoznak ugyanazzal a egyszerű felhasználónévvel (UPN). Az új fiók egy másik PUID (Passport Unique ID) érték kel jön létre. Amikor a felhasználó megpróbál hozzáférni egy webhelycsoporthoz vagy a OneDrive-hoz, a felhasználó nem megfelelő PUID azonosítóval rendelkezik. A második forgatókönyv a címtár-szinkronizálás az Active Directory szervezeti egységgel (OU). Ha a felhasználók már bejelentkeztek a SharePointba, majd áthelyezték őket egy másik szervezeti egységbe, és újraszinkronizálták őket a SharePointtal, akkor ezt a problémát tapasztalhatják.

A probléma megoldásához állítsa vissza az eredeti felhasználói felületet a [Microsoft 365 felhasználójának visszaállítása](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)című cikkben ismertetett lépésekkel.

Megjegyzés: Ha egy OneDrive vagy SharePoint Felügyeleti központ nem érhető el több olyan felhasználó számára, akinek korábban hozzáférése volt, előfordulhat, hogy ideiglenes szolgáltatásprobléma lépett fel.  [Ellenőrizze a szolgáltatás állapotának irányítópultját.](https://portal.office.com/adminportal/home#/servicehealth)


