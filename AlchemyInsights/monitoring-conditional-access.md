---
title: Feltételes hozzáférés figyelése
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702905"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Feltételes hozzáférés figyelése az Exchange-ben

A feltételes hozzáféréssel célzott felhasználók értesítést kapnak e-mailben, ha nem felelnek meg a szervezet hozzáférési követelményeinek. A probléma megoldásához az alábbi megoldások közül legalább egyet ajánlunk:
  
- Ha az eszköz feltételezetten regisztrált, értesítse a felhasználót, hogy nyissa meg a vállalati portál alkalmazást, és ellenőrizze, hogy megjelenik-e a vállalati portálon. Ha nem, akkor a felhasználónak regisztrálnia kell az eszközt.
    
- Az Azure portálon nyissa meg a **Intune \> eszköz megfelelősége**című részt. A **monitor** csoportban kattintson az **eszköz megfelelősége**elemre. Tekintse meg az eszköz megfelelőségi jelentését annak ellenőrzéséhez, hogy a felhasználó eszközének megfelelően van-e megjelölve. 
    
- Az Azure portálon nyissa meg a **Intune \> eszköz megfelelősége**című részt. A **kezelés**csoportban kattintson a **házirendek**elemre. Ellenőrizze, hogy a megfelelőségi házirendek listája tartalmazza-e a felhasználói eszközhöz tartozó profilt. Ha nincs kiosztva profil, akkor a Intune nem fogja tudni ellenőrizni az eszköz megfelelőségi állapotát. 
    
- Módosítsa a felhasználó feltételes hozzáférés-hozzárendelését.
    
1. Az Azure portálon nyissa meg az **Intune \> feltételes hozzáférési \> házirendeket**
    
2. Házirend kijelölése a listából
    
3. Kattintson **a felhasználók és csoportok** elemre.
    
4. Ha egy bizonyos házirendet valakinek szeretne célozni, vegye fel őket a **belefoglalási** listára. Ha meg szeretne győződni arról, hogy egy személy nincs kihagyva a házirendből, vegye fel őket a **kizárási** listára. 
    
További információ: [feltételes hozzáférésű eszközök figyelése](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

