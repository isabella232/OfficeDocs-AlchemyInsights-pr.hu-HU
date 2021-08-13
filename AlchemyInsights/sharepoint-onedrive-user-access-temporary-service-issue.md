---
title: Teljesítménybeli problémák SharePoint problémák OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093737"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint vagy OneDrive, Nem érhető el vagy Nem érhető el több felhasználó számára

Ha egy OneDrive vagy SharePoint nem érhető el több, korábban hozzáféréssel rendelkező felhasználó számára, átmeneti szolgáltatás-probléma lehet. [Ellenőrizze a szolgáltatás állapot-irányítópultját.](https://portal.office.com/adminportal/home#/servicehealth)

**Felhasználó hozzáadása és licencel**

Győződjön meg arról, hogy licenceket rendel a [felhasználókhoz Microsoft 365 Vállalati verzióban.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Engedélyek hozzárendelése**

Ha a felhasználóhoz hozzárendelt egy SharePoint-licencet, és továbbra is "hozzáférés megtagadva" üzenetet kap, ellenőrizze, hogy rendelkezik-e a megfelelő [jogosultsági szinttel.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**Fontolja meg a hozzáférési kérelem funkció használatának megfontolását**

A [hozzáférés-kérelmező funkcióval](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) a felhasználók hozzáférést kérhetnek olyan tartalmakhoz, amelyekhez jelenleg nincs engedélyük.

**Az egyéni parancsfájlok engedélyezése hozzáférés-megtagadó problémákat okozhat**

Bizonyos esetekben előfordulhat,  hogy az Egyéni parancsfájlok engedélyezése funkció hozzáférés-megtagadásról ad lehetőséget. Az érintett szolgáltatások listája biztonsági szempontokat és a funkció letiltására vonatkozó lehetőséget tartalmazza. Kérjük, keresse fel az Egyéni parancsfájl [engedélyezése vagy megakadályozása lehetőséget.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

