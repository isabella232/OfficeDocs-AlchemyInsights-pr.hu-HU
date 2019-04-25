---
title: Külső csoportok letiltása
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399593"
---
# <a name="how-to-disable-external-groups"></a>Külső csoportok letiltása

Yammer külső üzenetküldő Exchange átviteli szabályok – (ETR), a proaktív vezérlők vállalati adatok megosztását, elkerülésére vonatkozik. Annak érdekében, hogy korlátozza a felhasználók külső csoportok létrehozását, kell konfigurálása az Exchange átviteli szabály (ETR), és állítsa be az Exchange átviteli szabály segítségével blokkolja a külső üzenetküldő Yammer. 
  
Exchange Online admin center szabály létrehozása után a következő lépésekkel állítsa be az ETR Yammer alkalmaz:
  
- Bejelentkezés Yammer ellenőrzött admin, és **admin center Yammer**, ugorjon a C **ontent és biztonsági \> biztonsági beállításokat.**
    
- A **Külső üzenetküldő**, válassza a **az Exchange Online Exchange közlekedési szabályok érvényesítése – (ETR) a Yammer.**
    
- Válassza a **Mentés** gombot. 
    
További tudnivalókért tanulmányozza a [külső üzenetküldő Exchange átviteli szabályok Yammer hálózati vezérlő](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  

