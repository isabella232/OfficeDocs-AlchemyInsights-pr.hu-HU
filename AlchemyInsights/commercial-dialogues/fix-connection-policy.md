---
title: Kapcsolati házirend kijavítás
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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888408"
---
# <a name="fix-connection-policy"></a>Kapcsolati házirend kijavítás

Az e-maileket biztonságosként jelöltük meg, és a felhasználó Beérkezett üzenetek mappájába kézbesítették, mert a forrás IP-cím biztonságosként lett megjelölve az alapértelmezett kapcsolatszűrő házirendben. A házirend áttekintéshez kövesse az alábbi lépéseket:

1. A Microsoft 365 Defender portálon a Házirendek szakaszban & e-mailes együttműködési házirendek & szabályok veszélyforrások elleni védelem című <https://security.microsoft.com/>  \>  \>  \>  **szakaszát.**

   Ha közvetlenül a **Levélszemét-szűrési házirendek** lapot kell használnia, használja a <https://security.microsoft.com/antispam> következőt: .

2. A **Levélszemét-szűrési házirendek** lapon a házirend nevére kattintva válassza ki a Kapcsolatszűrő házirend **(alapértelmezett)** házirendet.

3. A megjelenő részleteket tartalmazó előgombra a Kapcsolatszűrés csoportban kattintson a Kapcsolatszűrő **házirend szerkesztése hivatkozásra.** 

4. Tekintse át Az alábbi **IP-címekről** vagy címtartományokról származó üzenetek engedélyezése mindig című szakasz bejegyzéseit, és ellenőrizze, hogy **be** van-e jelölve a Megbízható lista engedélyezése jelölőnégyzet.

   > [!NOTE]
   > A Microsoft előfizet a megbízható feladók külső forrásaira. Ha a megbízható feladók listája engedélyezve van, ezek a megbízható feladók nem lesznek tévesen levélszemétként megjelölve. Ezt a beállítást javasoljuk, mert ezzel csökkenti a vak pozitív üzenetek számát (a levélszemétként osztályozott e-mailek számát).

További információ: [Kapcsolatszűrés konfigurálása.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
