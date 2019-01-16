---
title: Felhasználói postafiók átalakítása megosztott postafiókjából?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28294120"
---
<span data-ttu-id="1f342-p101">Csak alakíthatja a felhasználói postafiók megosztott postafiókjából, ha a felhasználónak az Exchange ügyféllicenc. A postaláda konvertálása után továbbra is megjelennek az aktív felhasználók listában, mivel ez a jegyzék tartalmazza a megosztott postafiókokhoz. Azonban a konvertált postafiók is jelennek meg a megosztott postaláda listájában.</span><span class="sxs-lookup"><span data-stu-id="1f342-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="1f342-p102">Ha a konvertálás sikertelen próbál konvertálni a postafiókhoz az Exchange felügyeleti konzol, a böngésző gyorsítótár és a cookie-k törlése, és próbálkozzon újra. Ha ez még mindig nem működik, próbálja meg a postafiókhoz az Exchange felügyeleti rendszerhéj átalakítás a következő parancs futtatásával:</span><span class="sxs-lookup"><span data-stu-id="1f342-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="1f342-107">Postaláda-átalakítás további információ érhető el [átalakítása megosztott postafiókjából felhasználói postafiókot](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="1f342-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
