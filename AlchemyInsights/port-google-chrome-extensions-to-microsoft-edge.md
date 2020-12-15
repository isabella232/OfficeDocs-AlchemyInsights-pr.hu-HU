---
title: Google Chrome-bővítmények portja a Microsoft Edge-be (króm)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677879"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="d46c6-102">Google Chrome-bővítmények portja a Microsoft Edge-be (króm)</span><span class="sxs-lookup"><span data-stu-id="d46c6-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="d46c6-103">A [Google Chrome-bővítmények a Microsoft Edge (króm)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)számára könnyen elérhetők.</span><span class="sxs-lookup"><span data-stu-id="d46c6-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="d46c6-104">A legtöbb esetben csak minimális módosítások szükségesek a Microsoft Edge-ben a bővítmények futtatásához.</span><span class="sxs-lookup"><span data-stu-id="d46c6-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="d46c6-105">A Google Chrome által támogatott, a bővítmény API-k és a manifest-kulcsok a Microsoft Edge-kóddal kompatibilisek.</span><span class="sxs-lookup"><span data-stu-id="d46c6-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="d46c6-106">A Microsoft Edge azonban nem támogatja a bővítmény API-kat a Chrome. GCM, a Chrome. Identity. getAccounts, a Chrome. Identity. getAuthToken és a Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="d46c6-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>