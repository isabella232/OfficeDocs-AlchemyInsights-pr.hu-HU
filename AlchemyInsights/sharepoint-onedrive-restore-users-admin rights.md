---
title: Az Access által a webhelyekkel kapcsolatos OneDrive Vállalati verzió elhárítása
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957795"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Az Access által a webhelyekkel kapcsolatos OneDrive Vállalati verzió elhárítása

Ez a probléma leggyakrabban akkor fordul elő, ha egy felhasználót törölnek és újra létrehoznak ugyanazokkal az egyszerű felhasználónévvel. Az új fiók egy másik PUID (Passport Unique ID) érték használatával jön létre. Amikor a felhasználó megpróbál elérni egy webhelycsoportot vagy a hozzácsat OneDrive, helytelen PUID azonosítót ad meg. A második forgatókönyv a címtár-szinkronizálást is magában foglalja egy Active Directory-szervezeti egységben. Ha a felhasználók már bejelentkeztek a SharePoint, majd egy másik szervezeti egységbe áthelyezik őket, és újraszinkronizációs SharePoint, akkor ez a probléma jelentkezhet.

1. A probléma megoldásához állítsa vissza az eredeti egyszerű felhasználószámot a Következő cikkben található lépésekkel: Felhasználó [visszaállítása a](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)Microsoft 365.
2. Ha nem tudja visszaállítani az eredeti felhasználót, a következő lépésekkel távolítsa el a régi felhasználót OneDrive webhelyről: Felhasználó eltávolítása [a felhasználói adatok listájáról.]() 
3. Miután ezt megtette, ellenőrizheti, hogy a felhasználó rendszergazdai jogokkal rendelkezik-e a OneDrive-webhelyhez. Ehhez kövesse a Rendszergazda hozzáadása a felhasználó saját webhelyéhez című [OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

A jogosultsági szintekről további információt A jogosultsági szintek ismertetése a [SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
