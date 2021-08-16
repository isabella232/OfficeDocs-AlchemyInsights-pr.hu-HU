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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988109"
---
# <a name="fix-connection-policy"></a>Kapcsolati házirend kijavítás

Az e-mail biztonságosként lett megjelölve, és a felhasználó postaládájába lett kézbesítve, mert a küldő IP-cím biztonságosként lett megjelölve a kapcsolatszűrő házirendben. A házirend áttekintéshez tegye a következőket:

1. Válassza a [Office 365 biztonsági & megfelelőségi központot,](https://go.microsoft.com/fwlink/p/?linkid=2077143)majd a Veszélyforrások elleni **védelem** házirend Levélszemét  >    >  [elleni központban.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Az Egyéni **lapon** válassza a Kapcsolatszűrő **házirend** lapjának Házirend **szerkesztése parancsát.**
3. Tekintse át az **IP Allow (Ip-cím engedélyezése)** listát. Nézze **meg, Széf a lista** engedélyezve van-e.

    > [!NOTE]
    > A Microsoft előfizet a megbízható feladók külső forrásaira. Ha **Széf lista** engedélyezve van, a megbízható feladókat a rendszer nem jelöli tévesen levélszemétként. Ezt a beállítást javasoljuk, mert ezzel csökkenti a tévesen pozitív (tévesen levélszemétként osztályozott) üzenetek számát.
