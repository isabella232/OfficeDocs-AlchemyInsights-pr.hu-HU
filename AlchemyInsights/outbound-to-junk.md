---
title: Kimenő e-mail a Levélszemét mappába
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 869cd3d9fb8e5fce291244e4a39754d074b11358
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511726"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="480bd-102">Kimenő e-mail a Levélszemét mappába</span><span class="sxs-lookup"><span data-stu-id="480bd-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="480bd-103">Ha azt látja, hogy a kimenő üzenetek levélszemétként vannak megjelölve, tegye a következő lépéseket:</span><span class="sxs-lookup"><span data-stu-id="480bd-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="480bd-104">Ha még nem tette meg, fontolja meg [a kimenő levélszemét-házirend-értesítések konfigurálását.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)</span><span class="sxs-lookup"><span data-stu-id="480bd-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="480bd-105">Az [üzenetkövetés](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) segítségével ellenőrizheti, hogy a kimenő üzenet **tartalmaz-e Spam** eseményértéket a további részletekkel: Magas **kockázatú kézbesítési készlet használata**.</span><span class="sxs-lookup"><span data-stu-id="480bd-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="480bd-106">Ezeknél az üzeneteknél ellenőrizze az üzenet tartalmát, hogy mi tekinthető levélszemétnek.</span><span class="sxs-lookup"><span data-stu-id="480bd-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="480bd-107">Az aláírások például sok felhasználó számára problémákat okozhatnak.</span><span class="sxs-lookup"><span data-stu-id="480bd-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="480bd-108">Ha több példa van a levélszemétként megjelölt jogos kimenő üzenetekre, nyisson meg egy támogatási jegyet, és kérje meg a támogatási ügynököt, hogy küldje el az üzeneteket hamis pozitívként a spamelemzőinknek.</span><span class="sxs-lookup"><span data-stu-id="480bd-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="480bd-109">Készüljön fel az összes üzenetfejlécet tartalmazó mintaüzenetek megadására.</span><span class="sxs-lookup"><span data-stu-id="480bd-109">Be prepared to provide sample messages that include all message headers.</span></span>
