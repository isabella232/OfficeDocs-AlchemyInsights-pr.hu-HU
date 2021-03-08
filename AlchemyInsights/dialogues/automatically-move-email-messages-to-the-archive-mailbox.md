---
title: E-mailek automatikus áthelyezése az archív postaládába
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525095"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>E-mailek automatikus áthelyezése az archív postaládába

Így állíthat be olyan házirendet, amely automatikusan áthelyezi a felhasználók régi e-mailjeit az archív postaládába:

1. Ha ellenőrizni &, hogy engedélyezve van-e egy archív postaláda a felhasználó számára, menjen a Biztonsági [**&-**](https://go.microsoft.com/fwlink/p/?linkid=2077143)és megfelelőségi adatirányítási  >    >   archívumba. Ha nem, a figyelmeztetésben kattintson az **Engedélyezés,** majd az **Igen** gombra.
2. Az [**Adatmegőrzési címkékkel > Exchange Felügyeleti központ > felügyeleti központot.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Válassza a + ikont, majd válassza az **automatikus alkalmazás a teljes postaládára.**
4. Nevezze el az adatmegőrzési címkét, és válassza az **Áthelyezés az archívumba lehetőséget.** Az adatmegőrzési időszakhoz adja meg a kívánt időt, például 90 napot. Kattintson a **Mentés** gombra.
5. Most hozzon létre egy adatmegőrzési házirendet: válassza az **adatmegőrzési** házirendeket, majd az ikont választva vegyen fel egy új házirendet.
6. Adjon nevet az adatmegőrzési házirendnek, majd kattintással és görgetéssel keresse meg és vegye fel az éppen létrehozott adatmegőrzési címkét. Kattintson a **Mentés** gombra.
7. Végül alkalmazza az adatmegőrzési házirendet a felhasználó postaládájában: az Exchange Felügyeleti központban maradva, a címzettek  >  **postaládáihoz.** Jelölje ki az összes felhasználót, akire alkalmazni szeretné a házirendet, majd válassza a **Szerkesztés** (ceruza) ikont.
8. A párbeszédpanelen kattintson a **postaláda-szolgáltatások elemre.** Az **Adatmegőrzési házirend** alatt alkalmazza a mentés > **házirendet.**
9. A házirend minden felhasználóra való alkalmazásával kapcsolatos utasításokat az Adatmegőrzési házirend alkalmazása [postaládákra.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
