---
title: 1491-keresés-nem-visszatérő-várt-eredmények
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510574"
---
# <a name="content-search-not-returning-expected-results"></a>A tartalomkeresés nem adja vissza a várt eredményeket

Ha a Microsoft 365 biztonsági & megfelelőségi központjából futtat tartalomkeresést, nem várt keresési eredményeket kaphat. Gondolja át a következő ket, amelyek hatással lehetnek a keresési eredményekre:

- **Tartalomhelyek és keresési feltételek:** Győződjön meg arról, hogy a megfelelő tartalomhelyeket és keresési feltételeket választotta. Ha nagy méretű keresést futtatott (sok helyen), fontolja meg, hogy több keresésre osztja fel.

- **Részben indexelt elemek**: A postaládákból származó [részben indexelt elemek](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) szerepelnek a becsült keresési eredmények között. A SharePoint és a OneDrive webhelyein lévő, részben indexelt elemek azonban nem szerepelnek a keresési becslésben.

- **Keresési hibák**: Nagyszámú (több mint 100 000 postaláda) postaládában keres, keresési hibákat kaphat, például CS008-009 és CS012-002 hibakódokkal). Ebben az esetben próbálkozzon újra a sikertelen tartalomhelyeket keresve. További információt ebben a [cikkben](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) talál.
