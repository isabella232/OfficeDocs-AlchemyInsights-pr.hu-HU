---
title: A SharePoint vagy a OneDrive használatakor a karbantartási üzenet írásvédett
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670834"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>A SharePoint vagy a OneDrive használatakor a karbantartási üzenet írásvédett

A SharePoint vagy a OneDrive használatakor a felhasználók **csak olvashatóan kapják meg a karbantartási** üzenetet, ha a következő esetek egyikét kísérli meg használni. 

-   Tervezett vagy aktív karbantartási tevékenység.  Ellenőrizze, hogy az [üzenetközpont](https://portal.office.com/adminportal/home#/messagecenter)segítségével navigáljon.
-   Nagy prioritású, aktív szolgáltatási incidens. Ellenőrizze, hogy van-e valamilyen tanácsadója/incidense a [szolgáltatás állapotának](https://portal.office.com/adminportal/home#/servicehealth)megfelelő navigálásban.
-   Egy kisebb automatikus gyógyulási forgatókönyv, amely a kiszolgálók váratlan eseményei miatt az esetlegesen 30 percnél rövidebbek lehetnek. 
    
    Ezek a kisebb visszanyerések esetén nincsenek üzenetközpont vagy szolgáltatás-egészségügyi bejegyzések, de a szokásostól nagyon hamar vissza kell térnie.

Nagyon néhány esetben azt tapasztaltuk, hogy a fenti három eset egyike az oka, és a szolgáltatás vissza lett állítva, de a felhasználók böngésző-gyorsítótára nem törlődik.

A webhelyre való navigálás előtt próbálkozzon a gyorsítótár kiürítésével.

1. A Microsoft Edge böngészőben válassza a **Beállítások**, majd az **Adatvédelem és biztonság**lehetőséget.
2. A **böngészés törlése**csoportban válassza ki **a törölni kívánt**elemet.
3. Jelölje ki a **cookie-k és a mentett webhely adatai**lehetőséget, és válassza a **Törlés**lehetőséget.

>[!Note] 
> Ezek a lépések eltérőek lehetnek más böngészők, például a Mozilla Firefox vagy a Google Chrome használatakor.

>[!Note] 
> Egy másik lehetőség az, hogy megnyitja a SharePoint-webhelyet vagy a OneDrive egy új InPrivate-ablakban.