---
title: Bérlői házirend kijavítása (művelet felülbírálása)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896077"
---
# <a name="fix-tenant-policy-action-override"></a>Bérlői házirend kijavítása (művelet felülbírálása)

Az üzenetre az egyik levélszemét-szűrési házirend hatással volt. A házirendek áttekintéshez kövesse az alábbi lépéseket:

1. A Microsoft 365 Defender portálon a Házirendek szakaszban & e-mailes együttműködési házirendek & szabályok veszélyforrások elleni védelem című <https://security.microsoft.com/>  \>  \>  \>  **szakaszát.**

   Ha közvetlenül a **Levélszemét-szűrési házirendek** lapot kell használnia, használja a <https://security.microsoft.com/antispam> következőt: .

2. A **Levélszemét-szűrési** házirendek lapon jelölje ki a házirendet a házirend nevére **kattintva** ( Típus: Egyéni levélszemét-szűrési házirend vagy Név a Levélszemét-szűrési bejövő házirend **(alapértelmezett)**).  
3. A megjelenő részleteket tartalmazó elő panelen válassza a **Műveletek csoport** Műveletek szerkesztése **parancsát.**
4. Az **Üzenetműveletek** szakaszban tekintse át a Levélszemét,  a Nagy megbízhatóságú **levélszemét,** az **Adathalászat** és a Nagy megbízhatóságú adathalászat beállítást, és ellenőrizze, hogy az alábbi értékek közül van-e kiválasztva: 
   - **X-fejléc hozzáadása**
   - **Tárgysor berakása szöveggel**
   - **Üzenet átirányítása e-mail címre**
   - **Üzenet törlése**
   - **Nincs művelet**

   Lehetséges, hogy a  Normál beállítások minden ügyfélre Exchange Online Védelmi szolgáltatás az üzenetet.

További információ: [Levélszemét-szűrési házirendek konfigurálása az EOP szolgáltatásban.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
