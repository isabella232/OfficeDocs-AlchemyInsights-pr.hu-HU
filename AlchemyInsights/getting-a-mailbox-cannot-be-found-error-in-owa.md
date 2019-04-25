---
title: Postafiók első 126 nem található hibaüzenet az OWA?
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 126
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: fe8119c300e99170da4f338f2420b1229ab24bea
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32400827"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Az első hiba nem található a weben Outlook postafiók?

Ha a **postaláda nem található a következő** hibaüzenet jelenik meg az Outlook programot a weben, az Outlook a weben való kapcsolódáshoz használt fiók nem rendelkezik az Exchange Online licencet, és ezért nincs postaláda a fiókjához társított. A rendszergazda is licenc hozzárendelése a fiók az alábbiak szerint:

1. Nyissa meg a [Microsoft 365 felügyeleti központ](https://portal.office.com/adminportal/home#/homepage) , és **aktív felhasználók**csoportban jelölje be a **felhasználó szerkesztése**.

2. Megnyitó **felhasználó szerkesztése** lapon jelölje ki a felhasználót. A megnyitó felhasználó tulajdonságlapon kattintson **terméklicencek**a **Szerkesztés** gombra.

3. **Terméklicencek** lapon válassza ki a megfelelő **helyre** értéket, és rendel hozzá, amely tartalmazza az Exchange Online licencet (a licenc részletes adatainak megtekintéséhez bontsa ki). Ha elkészült, kattintson a **Mentés** gombra.
