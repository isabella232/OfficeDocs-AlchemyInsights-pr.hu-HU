---
title: Kimenő e-mailek a Levélszemét mappába
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769185"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="042a8-102">Kimenő e-mailek a Levélszemét mappába</span><span class="sxs-lookup"><span data-stu-id="042a8-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="042a8-103">Ha a kimenő üzeneteket levélszemétként jelöli meg, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="042a8-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="042a8-104">Ha még nem tette meg, fontolja meg a [kimenő levélszemét-házirend bejelentéseinek beállítását](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="042a8-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="042a8-105">Az [üzenet nyomon követése](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) szolgáltatással megtekintheti, hogy a kimenő üzenet a **Levélszemét** esemény értékét tartalmazza-e a további részletekkel: **nagy kockázatú kézbesítési készlet használata**.</span><span class="sxs-lookup"><span data-stu-id="042a8-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="042a8-106">Ha ezeket az üzeneteket szeretné ellenőrizni, tekintse át az üzenet tartalmát, hogy mi tekinthető levélszemétnek.</span><span class="sxs-lookup"><span data-stu-id="042a8-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="042a8-107">Az aláírások például olykor problémákat okozhatnak sok felhasználó esetében.</span><span class="sxs-lookup"><span data-stu-id="042a8-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="042a8-108">Ha a levélszemétként megjelölt megbízható kimenő üzenetekre több példa is van, nyisson meg egy támogatási jegyet, és kérje meg a támogatási ügynököt, hogy a levélszemét-elemzők számára téves pozitívként nyújtsa be az üzeneteket.</span><span class="sxs-lookup"><span data-stu-id="042a8-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="042a8-109">Készüljön fel az összes üzenet fejlécét tartalmazó minta üzenetek nyújtására.</span><span class="sxs-lookup"><span data-stu-id="042a8-109">Be prepared to provide sample messages that include all message headers.</span></span>
