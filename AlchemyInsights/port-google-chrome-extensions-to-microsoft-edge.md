---
title: Google Chrome-bővítmények portja a Microsoft Edge-be (Chromium)
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
- "8297"
- "9004617"
ms.openlocfilehash: 1c71d74d01c1e38e4c7789aea2c0b43701b3a5de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505286"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Google Chrome-bővítmények portja a Microsoft Edge-be (Chromium)

A Google Chrome bővítményei egyszerűen áthordhatóak a [Microsoft Edge-be (Chromium).](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension) A legtöbb esetben csak minimális módosításokra van szükség a bővítmények Microsoft Edge-ben való futtatásához.

A Google Chrome által támogatott mellék API-k és jegyzékfájlkulcsok a Microsoft Edge-sel kompatibilis kódokkal kompatibilisek. A Microsoft Edge azonban nem támogatja a chrome.gcm, a chrome.identity.getAccounts, a chrome.identity.getAuthToken és a chrome.instanceID kiterjesztést.