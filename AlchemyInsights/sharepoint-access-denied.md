---
title: Hozzáférés megtagadott üzenetekkel kapcsolatos hibák elhárítása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: af0bc0215f8feacc28a0b9bdf6b2659778736d669f7a3ff17628401e23d5fb6f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957975"
---
# <a name="troubleshoot-access-denied-messages"></a>Hozzáférés megtagadott üzenetekkel kapcsolatos hibák elhárítása

Ha egy SharePoint Online-webhely tallózása közben "hozzáférés megtagadva" üzenetet kap, olvassa el az alábbi cikkeket.

**Felhasználó hozzáadása és licencel**

Győződjön meg arról, hogy licenceket rendel a [felhasználókhoz Microsoft 365 Vállalati verzióban.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)

**Engedélyek hozzárendelése**

Ha a felhasználóhoz hozzárendelt egy SharePoint-licencet, és továbbra is "hozzáférés megtagadva" üzenetet kap, ellenőrizze, hogy rendelkezik-e a megfelelő jogosultsági [szinttel.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**Fontolja meg a hozzáférési kérelem funkció használatának megfontolását**

A [hozzáférés-kérelmező](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) funkcióval a felhasználók hozzáférést kérhetnek olyan tartalmakhoz, amelyekhez jelenleg nincs engedélyük. 

**Az egyéni parancsfájlok engedélyezése hozzáférés-megtagadó problémákat okozhat**

Bizonyos esetekben előfordulhat, hogy az "Egyéni parancsfájlok engedélyezése" funkció nem engedélyezi a hozzáférést. Az érintett szolgáltatások listája biztonsági szempontokat és a funkció letiltására vonatkozó lehetőséget tartalmazza. Kérjük, látogasson el az egyéni [parancsfájlok engedélyezése vagy megakadályozása webhelyre.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

Megjegyzés: Ha egy OneDrive vagy SharePoint nem érhető el több, korábban hozzáféréssel rendelkező felhasználó számára, átmeneti szolgáltatás-probléma lehet. [Ellenőrizze a szolgáltatás állapot-irányítópultját.](https://portal.office.com/adminportal/home#/servicehealth)


  

