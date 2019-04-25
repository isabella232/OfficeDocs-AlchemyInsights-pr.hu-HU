---
title: Felhasználói postafiók átalakítása megosztott postafiókjából?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374325"
---
Csak alakíthatja a felhasználói postafiók megosztott postafiókjából, ha a felhasználónak az Exchange ügyféllicenc. A postaláda konvertálása után továbbra is megjelennek az aktív felhasználók listában, mivel ez a jegyzék tartalmazza a megosztott postafiókokhoz. Azonban a konvertált postafiók is jelennek meg a megosztott postaláda listájában. 
  
Ha a konvertálás sikertelen próbál konvertálni a postafiókhoz az Exchange felügyeleti konzol, a böngésző gyorsítótár és a cookie-k törlése, és próbálkozzon újra. Ha ez még mindig nem működik, próbálja meg a postafiókhoz az Exchange felügyeleti rendszerhéj átalakítás a következő parancs futtatásával:
  
```
Set-Mailbox -Type Shared
```

Postaláda-átalakítás további információ érhető el [átalakítása megosztott postafiókjából felhasználói postafiókot](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
