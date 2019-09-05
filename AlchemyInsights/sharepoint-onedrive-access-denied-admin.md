---
title: Hozzáférés-megtagadási üzenetek – problémamegoldás
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751278"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>A SharePoint/OneDrive Admin Center rendszerben található hozzáférés-megtagadási üzenetek – problémamegoldás

Ha a SharePoint/OneDrive Admin Center webhely megnyitásakor hozzáférés-megtagadási üzenetet kap, akkor ellenőrizze, hogy [a felhasználóhoz rendel](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)-e licencet. Ha a felhasználó rendelkezik licenccel, győződjön meg arról is, hogy hozzá vannak-e [rendelve rendszergazdai szerepkör](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , amely hozzáfér az adminisztrációs központokhoz.

Ez a probléma akkor is előfordulhat, ha egy felhasználót töröl, és ugyanazzal az egyszerű felhasználónévvel (UPN) újra létrehozza. Az új fiók a Passport egyedi AZONOSÍTÓI értékének használatával jön létre. Mikor a felhasználó megpróbál-hoz belépés egy telek gyűjtemény vagy-uk OneDrive, a felhasználó birtokol egy rossz PUID. A második forgatókönyv egy Active Directory szervezeti egységgel (OU) rendelkező címtár-szinkronizálást foglal magában. Ha a felhasználók már bejelentkezett a SharePoint-ba, majd egy másik szervezeti egységbe kerülnek, és újra átviszik a SharePoint-alkalmazással, akkor a problémát tapasztalhatják.

A probléma megoldásához állítsa vissza az eredeti UPN-t a cikkben leírt lépésekkel, [állítsa vissza a felhasználót az Office 365-ben](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Jegyzék Ha egy OneDrive vagy SharePoint admin központ van nem elérhető-hoz sokszoros használók ki korábban belépés, ott május lenni egy ideiglenes szolgáltatás kérdés.  [Ellenőrizze a szolgáltatás állapotirányítópultját](https://portal.office.com/adminportal/home#/servicehealth).


