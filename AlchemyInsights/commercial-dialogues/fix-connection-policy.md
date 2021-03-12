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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746750"
---
# <a name="fix-connection-policy"></a>Kapcsolati házirend kijavítás

Az e-mail biztonságosként lett megjelölve, és a felhasználó postaládájába lett kézbesítve, mert a küldő IP-cím biztonságosként lett megjelölve a kapcsolatszűrő házirendben. A házirend áttekintéshez tegye a következőket:

1. Az [Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)Biztonsági & megfelelőségi központban, majd a Veszélyforrások elleni **védelem** házirend levélszemét  >    >  [elleni területén.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Az Egyéni **lapon** válassza a Kapcsolatszűrő **házirend** lapjának Házirend **szerkesztése parancsát.**
3. Tekintse át az **IP Allow (Ip-cím engedélyezése)** listát. Nézze **meg, hogy engedélyezve van-e** a Megbízható lista beállítás.

    > [!NOTE]
    > A Microsoft előfizet a megbízható feladók külső forrásaira. Ha **a Megbízható lista** engedélyezve van, a megbízható feladók nem lesznek tévesen levélszemétként megjelölve. Ezt a beállítást javasoljuk, mert ezzel csökkenti a tévesen pozitív (tévesen levélszemétként osztályozott) üzenetek számát.
