---
title: Több aktív munkamenet ugyanabba a postaládába
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: d2fd3f20346012baed21efd4900ca4cf73391d91
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439198"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="8f491-102">Több aktív munkamenet ugyanabba a postaládába</span><span class="sxs-lookup"><span data-stu-id="8f491-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="8f491-103">Az Exchange-erőforrások használatának szabályozásához a postaládának "költségvetése" van.</span><span class="sxs-lookup"><span data-stu-id="8f491-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="8f491-104">A költségvetésen felüli kivételt a következő körülmények válthatják ki, de nem kizárólagosan:</span><span class="sxs-lookup"><span data-stu-id="8f491-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="8f491-105">Ugyanabban az Outlook Web App-munkamenetben néhány böngészőlap nyílik meg.</span><span class="sxs-lookup"><span data-stu-id="8f491-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="8f491-106">Néhány aktív Outlook Web App-munkamenet ugyanarra a postaládára.</span><span class="sxs-lookup"><span data-stu-id="8f491-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="8f491-107">Néhány más ügyfélalkalmazás (Outlook, Outlook Mobile, egy harmadik féltől származó ügyfélalkalmazás) egyszerre fér hozzá a postaládához.</span><span class="sxs-lookup"><span data-stu-id="8f491-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="8f491-108">A hosszú ideig futó műveletek, például a keresési kérelmek végrehajtása egy másik aktív postaláda-munkamenetből történik.</span><span class="sxs-lookup"><span data-stu-id="8f491-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

