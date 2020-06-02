---
title: Az Access által a OneDrive Vállalati verzió webhelyeire irányuló üzenetek hibáinak elhárítása
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511186"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Az Access által a OneDrive Vállalati verzió webhelyeire irányuló üzenetek hibáinak elhárítása

Ez a probléma leggyakrabban akkor fordul elő, ha egy felhasználót törölnek, és újra létrehoznak ugyanazzal az egyszerű felhasználónévvel (UPN). Az új fiók egy másik PUID (Passport Unique ID) érték kel jön létre. Amikor a felhasználó megpróbál hozzáférni egy webhelycsoporthoz vagy a OneDrive-hoz, a felhasználó nem megfelelő PUID azonosítóval rendelkezik. A második forgatókönyv a címtár-szinkronizálás az Active Directory szervezeti egységgel (OU). Ha a felhasználók már bejelentkeztek a SharePointba, majd áthelyezték őket egy másik szervezeti egységbe, és újraszinkronizálták őket a SharePointtal, akkor ezt a problémát tapasztalhatják.

1. A probléma megoldásához állítsa vissza az eredeti felhasználói felületet a cikkben ismertetett lépésekkel, a Felhasználó visszaállítása a [Microsoft 365 alkalmazásban](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ha nem tudja visszaállítani az eredeti felhasználót, távolítsa el a régi felhasználót a OneDrive-webhelyről az alábbi lépésekkel, [távolítsa el a felhasználót a felhasználói adatok listájából](). 
3. Miután ez megtörtént, ellenőrizheti, hogy a felhasználó rendszergazdai jogokkal rendelkezik-e a OneDrive-webhelyen, ha a [Rendszergazda hozzáadása a felhasználó OneDrive-jához](https://docs.microsoft.com/sharepoint/manage-user-profiles) című lépéseit követve ellenőrzi.

A jogosultsági szintekről a [SharePoint engedélyszintjeinek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels)című cikkben olvashat bővebben.
