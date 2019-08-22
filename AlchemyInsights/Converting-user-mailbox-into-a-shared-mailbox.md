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
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496401"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>A felhasználói postafiók átalakítása megosztott postafiók

Csak alakíthatja a felhasználói postafiók megosztott postafiókjából, ha a felhasználónak az Exchange ügyféllicenc. A postaláda konvertálása után továbbra is megjelennek az aktív felhasználók listában, mivel ez a jegyzék tartalmazza a megosztott postafiókokhoz. Azonban a konvertált postafiók is jelennek meg a megosztott postaláda listájában. 
  
Ha a konvertálás sikertelen próbál konvertálni a postafiókhoz az Exchange felügyeleti konzol, a böngésző gyorsítótár és a cookie-k törlése, és próbálkozzon újra. Ha ez még mindig nem működik, próbálja meg a postafiókhoz az Exchange felügyeleti rendszerhéj átalakítás a következő parancs futtatásával:
  
```
Set-Mailbox -Type Shared
```

Postaláda-átalakítás további információ érhető el [átalakítása megosztott postafiókjából felhasználói postafiókot](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
