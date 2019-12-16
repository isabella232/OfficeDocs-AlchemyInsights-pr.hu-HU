---
title: Az OneDrive for Business webhelyeknek való hozzáférés megtagadási problémáinak elhárítása
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051607"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Az OneDrive for Business webhelyeknek való hozzáférés megtagadási problémáinak elhárítása

Ez a probléma leggyakrabban akkor jelentkezik, ha egy felhasználó törlődik, és ugyanazzal az egyszerű felhasználónévvel (UPN) újra létrehozza. Az új fiók a Passport egyedi AZONOSÍTÓI értékének használatával jön létre. Mikor a felhasználó megpróbál-hoz belépés egy telek gyűjtemény vagy-uk OneDrive, a felhasználó birtokol egy rossz PUID. A második forgatókönyv egy Active Directory szervezeti egységgel (OU) rendelkező címtár-szinkronizálást foglal magában. Ha a felhasználók már bejelentkezett a SharePoint-ba, majd egy másik szervezeti egységbe kerülnek, és újra átviszik a SharePoint-alkalmazással, akkor a problémát tapasztalhatják.

1. A probléma megoldásához állítsa vissza az eredeti UPN-t a cikk lépéseinek segítségével, a [felhasználó visszaállítása az Office 365-ben](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Ha Ön nem tud visszaad a eredeti felhasználó Önnek kellene eltávolít a régi felhasználó-ból OneDrive telek használ ezek lép, [eltávolít egy felhasználó-ból felhasználó értesít oldalra dől](). 
3. Után ez megtett, tudod igazol a felhasználó birtokol admin jogok-hoz OneDrive telek mellett alábbiak a lép-hoz [összead admins ' részére egy használók ' OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

A jogosultsági szintekkel kapcsolatos további tudnivalókért tanulmányozza a [SharePoint rendszerben a jogosultsági szintek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels)című témakört.
