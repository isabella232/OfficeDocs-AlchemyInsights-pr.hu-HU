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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694167"
---
# <a name="fix-connection-policy"></a>Kapcsolati házirend kijavítás

Az e-mail biztonságosként lett megjelölve, és a felhasználó beérkezett üzenetek mappájába lett kézbesítve, mert a küldéshez szükséges IP-címet a Kapcsolatszűrő házirend biztonságosként jelölte meg. A házirend áttekintéshez tegye a következőket:

1. Válassza az [Office 365 Biztonsági & megfelelőségi központot,](https://go.microsoft.com/fwlink/p/?linkid=2077143)majd a   >  Veszélyforrás-kezelési **házirend** levélszemét elleni  >  [védelem szolgáltatását.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Az Egyéni **lapon** válassza a Kapcsolatszűrő **házirendet,** majd a Házirend **szerkesztése lehetőséget.**
3. Tekintse át az **IP Allow (Ip Engedélyezése)** listát. Nézze **meg, hogy engedélyezve van-e** a megbízható lista.

    > [!NOTE]
    > A Microsoft előfizet a megbízható feladók külső forrásaira. Ha **a Megbízható feladók** lista engedélyezve van, a megbízható feladók nem lesznek tévesen levélszemétként megjelölve. Azt javasoljuk, hogy ezt a beállítást válassza, mert ezzel csökkenti a kapott hamis pozitív üzenetek (levélszemétként osztályozott) számát.
