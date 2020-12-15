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
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Google Chrome-bővítmények portja a Microsoft Edge-be (króm)

A [Google Chrome-bővítmények a Microsoft Edge (króm)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)számára könnyen elérhetők. A legtöbb esetben csak minimális módosítások szükségesek a Microsoft Edge-ben a bővítmények futtatásához.

A Google Chrome által támogatott, a bővítmény API-k és a manifest-kulcsok a Microsoft Edge-kóddal kompatibilisek. A Microsoft Edge azonban nem támogatja a bővítmény API-kat a Chrome. GCM, a Chrome. Identity. getAccounts, a Chrome. Identity. getAuthToken és a Chrome. instanceID.