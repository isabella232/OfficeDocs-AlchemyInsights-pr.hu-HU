---
title: Teljesítménnyel kapcsolatos problémák – SharePoint vagy OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771246"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>A SharePoint vagy a OneDrive lassú, elérhetetlen vagy nem elérhető több felhasználó esetében

Ha egy OneDrive vagy SharePoint-webhely nem érhető el több olyan felhasználónál, aki korábban hozzáféréssel rendelkezik, előfordulhat, hogy ideiglenes szolgáltatási probléma van. [Ellenőrizze a szolgáltatás állapota irányítópultot](https://portal.office.com/adminportal/home#/servicehealth).

**A felhasználó hozzáadása és licence**

Győződjön meg arról, hogy [licenceket rendel a felhasználókhoz a Microsoft 365 vállalati](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)verziójában.


**Engedélyek hozzárendelése**

Ha a felhasználó SharePoint-licenccel rendelkezik, és továbbra is egy hozzáférés-megtagadási üzenetet kap, győződjön meg arról, hogy rendelkeznek a [megfelelő jogosultsági szinttel](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**A hozzáférés kérése funkció használata**

A [hozzáférési kérés funkció](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) lehetővé teszi, hogy a felhasználók hozzáférést kérjen olyan tartalmakhoz, amelyekre jelenleg nincs engedélye.

**Hozzáférés megtagadását okozó egyéni parancsfájlok engedélyezése**

Bizonyos esetekben az *egyéni parancsfájl engedélyezése* funkció a hozzáférés megtagadását okozhatja. Az érintett szolgáltatások listáját, a biztonsági megfontolásokat és a funkció letiltását is lehetővé teszi. Kérjük, keresse meg az [egyéni parancsfájlok engedélyezése vagy letiltása című leírást](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

