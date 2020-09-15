---
title: A OneDrive vállalati verziós webhelyekhez való hozzáférés megtagadását jelző üzenetek hibaelhárítása
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
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670618"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>A OneDrive vállalati verziós webhelyekhez való hozzáférés megtagadását jelző üzenetek hibaelhárítása

Ez a probléma leggyakrabban akkor fordul elő, ha egy felhasználó törlődik, és a felhasználó ugyanazzal a egyszerű névvel (UPN) jön létre újra. Az új fiókot egy másik PUID (Passport egyedi azonosító) használatával hozza létre. Amikor a felhasználó megkísérel hozzáférni egy webhelycsoportban vagy a OneDrive, a felhasználó helytelen PUID rendelkezik. A második forgatókönyv a címtár-szinkronizálást jelenti Active Directory-beli szervezeti egységgel (OU). Ha a felhasználók már bejelentkezett a SharePointba, és egy másik szervezeti egységbe vannak áthelyezve, és a SharePointtal újra szinkronizálják őket, előfordulhat, hogy ez a probléma tapasztalható.

1. A probléma megoldásához vissza kell állítania az eredeti UPN-t a cikkben ismertetett lépésekkel, ha [vissza szeretne állítani egy felhasználót a Microsoft 365-ban](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ha nem tudja visszaállítani az eredeti felhasználót, a fenti lépésekkel távolítsa el a régi felhasználót a OneDrive webhelyről, [távolítsa el a felhasználót a felhasználói adatok listából](). 
3. Miután ezt megtette, ellenőrizheti, hogy a felhasználó rendszergazdai jogosultságokkal rendelkezik-e a OneDrive-webhelyhez a [rendszergazda hozzáadása a felhasználó OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) című témakör lépéseit követve.

A jogosultsági szintekről a [SharePoint jogosultsági szintjeinek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels)című témakörben olvashat bővebben.
