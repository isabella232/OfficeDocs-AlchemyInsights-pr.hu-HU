---
title: Csoport létrehozása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816358"
---
# <a name="create-a-group"></a>Csoport létrehozása

Ez a témakör a csoportok létrehozását ismerteti.

**Csoport létrehozására vonatkozó engedély**

Győződjön meg arról, hogy jogosult új csoport létrehozására. A globális rendszergazdák letilthatják a csoportok létrehozását az Azure Portal webhelyen vagy az Access panelen. Szükség lehet egy rendszergazdára az új csoport létrehozásához vagy a megfelelő engedélyek létrehozására.

**Csoport létrehozási engedélyeinek kezelése**

1. A globális rendszergazdák kezelhetik a csoportok létrehozásának engedélyét (biztonsági okokból) vagy az Azure Portal vagy a Hozzáférési panelen létrehozott Office 365-csoportokat "A felhasználók biztonsági csoportokat hozhatnak létre az Azure Portálon" vagy a "Felhasználók létrehozhatnak Office 365-csoportokat az Azure Portals webhelyen" lehetőséget választva a Minden csoport általános  >  **(Beállítások)** csoportjában.
2. Ha Azure Active Directory P1 Premium-licenccel rendelkezik, korlátozhatja a csoportok létrehozását úgy is, hogy csak egy felhasználócsoportot jelöljön ki.

**Az office 365-csoport új tagjainak üdvözlő értesítésének letiltása**

Az Office 365-csoportokba felvett felhasználóknak küldött üdvözlő értesítés letiltható, ha a Powershellben az **UnifiedGroupWelcomeMessageEnabled** beállítást False (Hamis) beállítással tiltja le. Erről a beállításról itt [olvashat.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

