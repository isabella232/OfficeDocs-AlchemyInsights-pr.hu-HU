---
title: Feltételes hozzáférés figyelése
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713720"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Az Exchange feltételes hozzáférésének figyelése

A feltételes hozzáféréssel rendelkező felhasználók értesítést kapnak e-mailben, ha nem felelnek meg a szervezet hozzáférési követelményeinek. A megoldáshoz az alábbi megoldások közül választhat:
  
- Ha az eszköz vélelmezni kell, hogy regisztrált, javasoljuk a felhasználónak, hogy menjen a Céges portál alkalmazást, és ellenőrizze, hogy megjelenik-e a céges portálon. Ha nem, a felhasználónak regisztrálnia kell az eszközt.
    
- Az Azure Portalon nyissa meg az **Intune-eszköz \> megfelelősége.** A **Figyelő** csoportban kattintson **az Eszközmegfelelőség**elemre. Tekintse meg az eszköz megfelelőségi jelentését, és ellenőrizze, hogy a felhasználó eszköze megfelelőként van-e megjelölve. 
    
- Az Azure Portalon nyissa meg az **Intune-eszköz \> megfelelősége.** A **Kezelés csoportban**kattintson a **Házirendek**gombra. A megfelelőségi szabályzatok listájában ellenőrizze, hogy egy profil hozzá van-e rendelve a felhasználó eszközéhez. Ha nincs hozzárendelve profil, akkor az Intune nem fogja tudni megerősíteni az eszköz megfelelőségi állapotát. 
    
- A felhasználó feltételes hozzáférési hozzárendelésének szerkesztése.
    
1. Az Azure Portalon nyissa meg az **Intune \> feltételes hozzáférési \> szabályzatait**
    
2. Házirend kiválasztása a listából
    
3. Kattintson **a Felhasználók és csoportok elemre.**
    
4. Ha egy bizonyos házirendet meg szeretne célozni valakire, vegye fel a **Belefoglalás listára.** Annak érdekében, hogy egy személy kikerüljön a házirendből, vegye fel őket a **Kizárás listára.** 
    
További információ: [A feltételes hozzáférésű eszközök figyelése](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

