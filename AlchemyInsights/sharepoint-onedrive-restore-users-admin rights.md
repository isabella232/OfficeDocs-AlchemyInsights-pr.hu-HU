---
title: Felhasználók hozzáférésének biztosítása a SharePoint és a OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736650"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Felhasználók hozzáférésének biztosítása a SharePoint és a OneDrive

Ez a probléma leggyakrabban akkor fordul elő, amikor a felhasználó törli, és újra létrehozza a ugyanolyan egyszerű felhasználónév (UPN). Az új fiók jön létre egy másik értéket PUID (Passport egyedi azonosító) segítségével. Ha a felhasználó megpróbál hozzáférni egy webhelycsoport vagy a OneDrive, a felhasználó rendelkezik egy helytelen PUID. A második forgatókönyv magában foglalja a könyvtár szinkronizálás az Active Directory szervezeti egységet (OU). Ha a felhasználó rendelkezik már bejelentkezett a SharePoint, majd átkerül egy másik szervezeti egység és SharePoint resynced, akkor ez a probléma tapasztalhatnak.

A probléma megoldásához a cikk[az Office 365 rendszerben a felhasználó visszaállítási](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide)lépéseket az eredeti UPN kell visszaállítani.

Miután ez elkészült, a felhasználó rendelkezik rendszergazdai jogokat a OneDrive webhelyen történő [hozzáadása admin által a felhasználó OneDrive a](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) lépéseket követve ellenőrizheti

Jogosultsági szintekkel kapcsolatos további tudnivalókért lásd a cikk [SharePoint jogosultsági szintek ismertetése](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
