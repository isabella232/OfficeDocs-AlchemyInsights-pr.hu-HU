---
title: A feltételes hozzáférésű figyelése
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418471"
---
# <a name="monitoring-conditional-access"></a>A feltételes hozzáférésű figyelése

Célzott feltételes hozzáféréssel rendelkező felhasználók kapnak értesítést e-mailben, ha nem felel meg a szervezet hozzáférési követelmények. Úgy oldhatja meg, ajánlott egy vagy több a következő oldatokat:
  
- Ha az eszköz feltételezhetőleg igényelt, tájékoztatja a felhasználót, hogy nyissa meg a vállalati portál app, és ellenőrizze, hogy a vállalati portál megjelenik. Ha nem, a felhasználó az eszközt kell igényelni.
    
- Az Azure portálon Ugrás **Intune \> eszköz való**. Kattintson a **Monitor** **eszköz betartását**. Ellenőrizze, hogy a felhasználó eszköz van megjelölve, kompatibilis az eszköz megfelelési jelentés megtekintése. 
    
- Az Azure portálon Ugrás **Intune \> eszköz való**. Kattintson a **Manage**, **házirendek**. Megfelelés irányelveinek listája ellenőrizze, hogy a profil a felhasználó eszköz van rendelve. Ha nincs profil van rendelve, majd Intune nem tudják megfelelési Eszközállapot megerősítéséhez. 
    
- A felhasználó a feltételes hozzáférésű hozzárendelés szerkesztése.
    
1. Az Azure portálon Ugrás **Intune \> a feltételes hozzáférésű \> politika**
    
2. Jelölje ki a szabályzatot a listán
    
3. Kattintson a **felhasználók és csoportok**
    
4. Valaki, egy bizonyos házirend célozza meg, vegye fel őket a **belefoglalási** listába felvenni. Annak érdekében, hogy egy személy a házirend nincs megadva, adja hozzá őket a **kizárása** listához. 
    
További: [hogyan Monitor feltételes hozzáférést biztosító eszközök](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

