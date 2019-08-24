---
title: Csak olvasásra szóló karbantartási jelenik meg, amikor próbál használni a SharePoint- vagy OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620725"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Csak olvasásra szóló karbantartási jelenik meg, amikor próbál használni a SharePoint- vagy OneDrive

Felhasználók is hibaüzenet **Írásvédett karbantartás** próbál használni a SharePoint- vagy OneDrive az alábbi esetek valamelyike. 

-   A tervezett és aktív karbantartási tevékenység.  Ellenőrizze, hogy azokat a [Message Center](https://portal.office.com/adminportal/home#/messagecenter)navigáljon.
-   Magas prioritású aktív szerviz esemény, amely felmerülhet. Ellenőrizze, hogy bármely tanácsadók eseményekre való [Egészségügyi szolgáltatás](https://portal.office.com/adminportal/home#/servicehealth).
-   Kisebb automatikus javító helyreállítás, a kiszolgálókon, amelyek kevesebb, mint 30 perc, vagy úgy lehet, hogy tart minden olyan váratlan események miatt sikerült előfordul. 
    
    Vannak a nem Message Center vagy egészségügyi szolgáltatás által használt ezek kisebb helyreállítást de vissza a normál nagyon legrövidebb időn belül.

Nagyon kevés alkalommal azt megfigyelhető, hogy a három fent említett esetek valamelyike okozhatta, és szolgáltatás visszaállította, de a felhasználók a böngésző gyorsítótár még nem lett bejelölve.

Meg kell kísérelni a böngésző gyorsítótár kiürítése előtt nyissa meg a webhelyet.

1. A Microsoft Edge böngészőben jelölje be a **Beállítások**, és válassza a **adatvédelmi és biztonsági**.
2. **Egyértelmű böngészés**csoportban **Válassza ki, milyen jelet**.
3. Jelölje be a **cookie-k és a mentett webhely adatokat**, és válassza a **világos**.

>[!Note] 
> Lépések eltérhetnek a más böngészőkben, például a Mozilla Firefox vagy Google Chrome használata során.

>[!Note] 
> Egy másik lehetőség az InPrivate-új ablakban nyílik meg a SharePoint-webhely vagy a OneDrive lenne.