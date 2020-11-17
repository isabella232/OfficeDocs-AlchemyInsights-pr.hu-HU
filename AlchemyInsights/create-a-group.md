---
title: Csoport létrehozása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088905"
---
# <a name="create-a-group"></a>Csoport létrehozása

Ez a témakör ismerteti a csoportok létrehozását.

**Csoport létrehozásának engedélye**

Ellenőrizze, hogy jogosult-e új csoport létrehozására. A globális rendszergazda letilthatja a csoportok létrehozását az Azure portálon vagy az Access-panelen. Előfordulhat, hogy a rendszergazdának létre kell hoznia az új csoportot, vagy megfelelő engedélyeket kell adnia.

**Csoport létrehozási engedélyeinek kezelése**

1. A globális rendszergazdák kezelhetik a csoport létrehozásához szükséges engedélyeket (biztonsági okokból kifolyólag) vagy az Azure portálon vagy az Access-munkaablakban létrehozott Office 365-csoportokat, ha a "felhasználók létrehozhatnak biztonsági csoportokat az Azure-portálokon" vagy a "felhasználók létrehozhatnak Office 365-csoportokat az Azure portálokon" az **összes csoport**  >  **általános (beállítások)** parancsára kattintva.
2. A csoportok létrehozását úgy is korlátozhatja, hogy a felhasználók egy csoportját kijelölje, ha az Azure Active Directory P1 prémium licenccel rendelkezik.

**Az új Office 365-csoporttagok üdvözlő értesítésének letiltása**

Az Office 365-csoportokba felvett felhasználóknak küldött üdvözlő értesítést a PowerShell **UnifiedGroupWelcomeMessageEnabled** false értékre állításával lehet letiltani. [Ebben a beállításban](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)tájékozódhat.

