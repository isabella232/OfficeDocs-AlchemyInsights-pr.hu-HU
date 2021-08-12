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
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929307"
---
# <a name="create-a-group"></a>Csoport létrehozása

Ez a témakör a csoportok létrehozását ismerteti.

**Csoport létrehozására vonatkozó engedély**

Győződjön meg arról, hogy jogosult új csoport létrehozására. A globális rendszergazdák letilthatják a csoportok létrehozását az Azure Portal webhelyen vagy az Access panelen. Szükség lehet egy rendszergazdára az új csoport létrehozásához vagy a megfelelő engedélyek létrehozására.

**Csoport létrehozási engedélyeinek kezelése**

1. A globális rendszergazdák a "Felhasználók hozhatnak létre biztonsági csoportokat az Azure Portal webhelyen vagy az Access panelen Office 365" vagy "A felhasználók biztonsági csoportokat hozhatnak létre az Azure Portálon" vagy "A felhasználók létrehozhatnak azure-portálon" lehetőséget választva kezelhetik Office 365 csoportok létrehozására vonatkozó engedélyeket az Összes csoportban – Általános  >  **(Gépház)** beállítással.
2. A csoport létrehozását korlátozhatja úgy is, hogy csak egy felhasználócsoportot jelöljön ki, Azure Active Directory P1 Prémium licenccel rendelkezik.

**A csoporttagok új Office 365 értesítésének letiltása**

A Office 365-csoportokba felvett felhasználóknak küldött üdvözlő értesítés letiltható az **UnifiedGroupWelcomeMessageEnabled** beállítást False értékre adva a Powershellben. Erről a beállításról itt [olvashat.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

