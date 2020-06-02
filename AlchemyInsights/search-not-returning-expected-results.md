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
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="9ec6a-102">A tartalomkeresés nem adja vissza a várt eredményeket</span><span class="sxs-lookup"><span data-stu-id="9ec6a-102">Content Search not returning expected results</span></span>

<span data-ttu-id="9ec6a-103">Ha a Microsoft 365 biztonsági & megfelelőségi központjából futtat tartalomkeresést, nem várt keresési eredményeket kaphat.</span><span class="sxs-lookup"><span data-stu-id="9ec6a-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="9ec6a-104">Gondolja át a következő ket, amelyek hatással lehetnek a keresési eredményekre:</span><span class="sxs-lookup"><span data-stu-id="9ec6a-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="9ec6a-105">**Tartalomhelyek és keresési feltételek:** Győződjön meg arról, hogy a megfelelő tartalomhelyeket és keresési feltételeket választotta.</span><span class="sxs-lookup"><span data-stu-id="9ec6a-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="9ec6a-106">Ha nagy méretű keresést futtatott (sok helyen), fontolja meg, hogy több keresésre osztja fel.</span><span class="sxs-lookup"><span data-stu-id="9ec6a-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="9ec6a-107">**Részben indexelt elemek**: A postaládákból származó [részben indexelt elemek](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) szerepelnek a becsült keresési eredmények között.</span><span class="sxs-lookup"><span data-stu-id="9ec6a-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="9ec6a-108">A SharePoint és a OneDrive webhelyein lévő, részben indexelt elemek azonban nem szerepelnek a keresési becslésben.</span><span class="sxs-lookup"><span data-stu-id="9ec6a-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="9ec6a-109">**Keresési hibák**: Nagyszámú (több mint 100 000 postaláda) postaládában keres, keresési hibákat kaphat, például CS008-009 és CS012-002 hibakódokkal).</span><span class="sxs-lookup"><span data-stu-id="9ec6a-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="9ec6a-110">Ebben az esetben próbálkozzon újra a sikertelen tartalomhelyeket keresve.</span><span class="sxs-lookup"><span data-stu-id="9ec6a-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="9ec6a-111">További információt ebben a [cikkben](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) talál.</span><span class="sxs-lookup"><span data-stu-id="9ec6a-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
