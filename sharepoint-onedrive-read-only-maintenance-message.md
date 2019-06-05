---
title: E-mailben kap egy TenantAccessBlockedException hiba elérésekor 127?
ms.author: kirks
author: Techwriter40
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
ms.openlocfilehash: 54ebc269b391e6b0d607e55af8283ebf3d9e2aa7
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715074"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Csak olvasásra szóló karbantartási jelenik meg, amikor próbál használni a SharePoint- vagy OneDrive

Jelenhet meg egy írásvédett karbantartási üzenet megkísérelte a SharePoint-vagy OneDrive.

Ellenőrizze, nincs-e <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>navigáljon a bérlő bekövetkező aktív karbantartás. Végezetül ellenőrizze, akkor látogassa meg a <a href="https://portal.office.com/adminportal/home#/servicehealth">Egészségügyi szolgáltatás</a> , amely felmerülhet tanácsadók/események ellenőrzése.

Ha sem az üzenet vagy szolgáltatás egészségügyi irányítópult tudomásul vették, aktuális karbantartási semmit a bérlő számára, ez lehet a böngésző gyorsítótár-probléma.

Meg kell kísérelni a böngésző gyorsítótár kiürítése előtt nyissa meg a webhelyet.

  <li>A Microsoft Edge böngészőben Ugrás <strong>több &hellip; &gt; beállítások</strong></li>  <li><strong>Egyértelmű böngészés </strong>csoportban <strong>Válassza ki, milyen jelet</strong>.</li>  <li>Válassza ki a cookie-k és a webhely mentett adatok jelölőnégyzetet, és válassza ki a <strong>törlése</strong>.</li>  </ol>  

**Megjegyzés**: ezeket a lépéseket más böngészőkben, például a Firefox vagy Chrome használata esetén eltérő lehet.

