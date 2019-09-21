---
title: Kimenő e-mailt a Levélszemét mappába
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 371d2c46e9048365fd343145330536bd9cf1db82
ms.sourcegitcommit: 1002f510fadb92c143cd6bbb60b42a851d5a38e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37062788"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="4539a-102">Kimenő e-mailt a Levélszemét mappába</span><span class="sxs-lookup"><span data-stu-id="4539a-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="4539a-103">Ha a kimenő üzeneteket levélszemétként jelöli meg, hajtsa a következő lépéseket:</span><span class="sxs-lookup"><span data-stu-id="4539a-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="4539a-104">Ha még nem tette meg, fontolja meg a [kimenő levélszemétre vonatkozó értesítések konfigurálását](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="4539a-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="4539a-105">Az [üzenetkövetés](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) segítségével ellenőrizze, hogy a kimenő üzenethez tartozik-e **Levélszemét** eseményérték a további részletek: **használjon magas kockázatú kézbesítési készletet**.</span><span class="sxs-lookup"><span data-stu-id="4539a-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="4539a-106">Ezeknél az üzeneteknél, ellenőrizze az üzenet tartalmát, hogy mit lehet levélszemétnek tekinteni.</span><span class="sxs-lookup"><span data-stu-id="4539a-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="4539a-107">Előfordulhat például, hogy az aláírások sok felhasználó számára okoznak problémát.</span><span class="sxs-lookup"><span data-stu-id="4539a-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="4539a-108">Ha van több példa a törvényes kimenő üzenetek, amelyek jelölése a szemét, nyisson meg egy támogatási jegyet, és kérje a támogatási megbízott, hogy küldje el az üzenetek hamis pozitívok, hogy a spam elemzők.</span><span class="sxs-lookup"><span data-stu-id="4539a-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="4539a-109">Készüljön fel az összes üzenet fejlécét tartalmazó mintaüzenetek biztosítására.</span><span class="sxs-lookup"><span data-stu-id="4539a-109">Be prepared to provide sample messages that include all message headers.</span></span>
