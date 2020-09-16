---
title: 1491 – keresés – vissza – a várt eredmények
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740476"
---
# <a name="content-search-not-returning-expected-results"></a>A tartalmi keresés nem tér vissza a várt eredményekre

Ha a Microsoft 365 biztonsági & megfelelőségi központból keres tartalmat, váratlan találatokat kaphat. Tekintse meg az alábbi, a találatokat befolyásoló dolgokat:

- **Tartalmi helyek és keresési feltételek**: Győződjön meg arról, hogy a megfelelő tartalmi helyeket és keresési feltételeket jelölte ki. Ha nagy kereséssel (sok hellyel) futott, fontolja meg több keresésre való felosztást.

- **Részlegesen indexelt elemek**: a postaládákban lévő  [részlegesen indexelt elemek](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) szerepelnek a becsült találatok között. A SharePoint és a OneDrive webhelyekről származó részlegesen indexelt elemek azonban nem szerepelnek a keresési becslésben.

- **Keresési hibák**: Ha nagy számú postaládában keres (több mint 100 000-postaládában), keresési hibákat kaphat, például a CS008-009 és a CS012-002. Ebben az esetben próbálkozzon újra a kereséssel a sikertelenül megjelenő tartalmi helyeken. További információt  [ebben a cikkben](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) talál.
