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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="c88e3-102">A felhasználói postafiók átalakítása megosztott postafiók</span><span class="sxs-lookup"><span data-stu-id="c88e3-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="c88e3-103">Csak alakíthatja a felhasználói postafiók megosztott postafiókjából, ha a felhasználónak az Exchange ügyféllicenc.</span><span class="sxs-lookup"><span data-stu-id="c88e3-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="c88e3-104">A postaláda konvertálása után továbbra is megjelennek az aktív felhasználók listában, mivel ez a jegyzék tartalmazza a megosztott postafiókokhoz.</span><span class="sxs-lookup"><span data-stu-id="c88e3-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="c88e3-105">Azonban a konvertált postafiók is jelennek meg a megosztott postaláda listájában.</span><span class="sxs-lookup"><span data-stu-id="c88e3-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="c88e3-106">Ha a konvertálás sikertelen próbál konvertálni a postafiókhoz az Exchange felügyeleti konzol, a böngésző gyorsítótár és a cookie-k törlése, és próbálkozzon újra.</span><span class="sxs-lookup"><span data-stu-id="c88e3-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="c88e3-107">Ha ez még mindig nem működik, próbálja meg a postafiókhoz az Exchange felügyeleti rendszerhéj átalakítás a következő parancs futtatásával:</span><span class="sxs-lookup"><span data-stu-id="c88e3-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="c88e3-108">Postaláda-átalakítás további információ érhető el [átalakítása megosztott postafiókjából felhasználói postafiókot](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c88e3-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
