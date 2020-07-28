---
title: Csapatok privát csatornájának törlése
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439326"
---
# <a name="delete-a-teams-private-channel"></a>Csapatok privát csatornájának törlése

A Microsoft nak tudomása van arról, hogy probléma van a Teams privát csatornáinak törlésével, ha az alapul szolgáló SharePoint-webhelyhez engedélyezve van a SharePoint-adatmegőrzési házirendek. A Microsoft dolgozik egy javításon. Addig is a következő kerülő megoldások segítségével törölheti a privát csatornát.

**A csoport-/webhelycsoport kizárása a SharePoint-adatmegőrzési szabályból.**

1. Nyissa meg az Office 365 felügyeleti portálját, és válassza az **Összes megjelenítése** lehetőséget a bal oldali navigációs ablakban.
2. A **Felügyeleti központok csoportban**nyissa meg **a Biztonsági &**  >  **megfelelőségi adatveszteség-megelőzési**  >  **házirendet.**
3. Azonosítsa a SharePoint-webhelyekre vonatkozó házirendeket, és módosítsa a házirendet úgy, hogy a privát csatornát tartalmazó csoport SharePoint-webhelye NE szerepeljen az adatmegőrzési szabályzatban.
4. Mentse a házirendet.
    A házirend-beállítások érvénybe léptetése akár 24 órát is igénybe vehet.
    A webhely kizárása után törölheti a privát csatornát.  
    
***Előfordulhat,*** hogy a Privát csatornát a Microsoft Teams segítségével törölheti Android-eszközén. 

A kapcsolódó SharePoint-információk a [Nem törölhetők elemek a SharePoint Online-ban vagy a OneDrive Vállalati verzióban](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)című témakörben olvashat.