---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052712"
---
# <a name="content-search-not-returning-expected-results"></a>A tartalomkeresés nem a várt eredményt adja

Ha a tartalomkeresést a megfelelőségi központ biztonsági Microsoft 365 biztonsági & futtatja, előfordulhat, hogy nem a várt találatokat kapja. Vegye figyelembe, hogy milyen hatással lehetnek a találatok:

- **Tartalomhelyek és keresési feltételek:** Győződjön meg arról, hogy a megfelelő tartalomhelyeket és keresési feltételeket választotta. Ha nagy keresést futtatott (sok helyen), érdemes több keresésre is felosonni.

- **Részben indexelt elemek:** A postaládákból részlegesen  [indexelt](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) elemek szerepelnek a becsült keresési eredmények között. A keresési becslés azonban SharePoint és OneDrive nem szerepel a webhelyek részleges indexelt elemei között.

- **Keresési hibák:** Nagyszámú (több mint 100 000 postaláda) postaládában való kereséskor keresési hibák jelenhetnek meg, például a CS008-009 és a CS012-002 hibakódok). Ebben az esetben csak a sikertelen tartalomhelyek keresését próbálja meg újból. További  [információt ebben](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) a cikkben talál.
