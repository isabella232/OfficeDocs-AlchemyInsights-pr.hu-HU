---
title: Hibaelhárítás a hozzáférés megtagadva a OneDrive üzenetek üzleti helyek
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 42a56b17e41649d979cf442909e8357eb262cf9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354799"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Hibaelhárítás a hozzáférés megtagadva a OneDrive üzenetek üzleti helyek

Ez a probléma leggyakrabban akkor fordul elő, amikor a felhasználó törli, és újra létrehozza a ugyanolyan egyszerű felhasználónév (UPN). Az új fiók jön létre egy másik értéket PUID (Passport egyedi azonosító) segítségével. Ha a felhasználó megpróbál hozzáférni egy webhelycsoport vagy a OneDrive, a felhasználó rendelkezik egy helytelen PUID. A második forgatókönyv magában foglalja a könyvtár szinkronizálás az Active Directory szervezeti egységet (OU). Ha a felhasználó rendelkezik már bejelentkezett a SharePoint, majd átkerül egy másik szervezeti egység és SharePoint resynced, akkor ez a probléma tapasztalhatnak.

A probléma megoldásához a cikk[az Office 365 rendszerben a felhasználó visszaállítási](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)lépéseket az eredeti UPN kell visszaállítani.

Miután ez elkészült, a felhasználó rendelkezik rendszergazdai jogokat a OneDrive webhelyen történő [hozzáadása admin által a felhasználó OneDrive a](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) lépéseket követve ellenőrizheti

Jogosultsági szintekkel kapcsolatos további tudnivalókért lásd a cikk [SharePoint jogosultsági szintek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
