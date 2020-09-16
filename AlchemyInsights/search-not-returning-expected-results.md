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
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="f0e23-102">A tartalmi keresés nem tér vissza a várt eredményekre</span><span class="sxs-lookup"><span data-stu-id="f0e23-102">Content Search not returning expected results</span></span>

<span data-ttu-id="f0e23-103">Ha a Microsoft 365 biztonsági & megfelelőségi központból keres tartalmat, váratlan találatokat kaphat.</span><span class="sxs-lookup"><span data-stu-id="f0e23-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="f0e23-104">Tekintse meg az alábbi, a találatokat befolyásoló dolgokat:</span><span class="sxs-lookup"><span data-stu-id="f0e23-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="f0e23-105">**Tartalmi helyek és keresési feltételek**: Győződjön meg arról, hogy a megfelelő tartalmi helyeket és keresési feltételeket jelölte ki.</span><span class="sxs-lookup"><span data-stu-id="f0e23-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="f0e23-106">Ha nagy kereséssel (sok hellyel) futott, fontolja meg több keresésre való felosztást.</span><span class="sxs-lookup"><span data-stu-id="f0e23-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="f0e23-107">**Részlegesen indexelt elemek**: a postaládákban lévő  [részlegesen indexelt elemek](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) szerepelnek a becsült találatok között.</span><span class="sxs-lookup"><span data-stu-id="f0e23-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="f0e23-108">A SharePoint és a OneDrive webhelyekről származó részlegesen indexelt elemek azonban nem szerepelnek a keresési becslésben.</span><span class="sxs-lookup"><span data-stu-id="f0e23-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="f0e23-109">**Keresési hibák**: Ha nagy számú postaládában keres (több mint 100 000-postaládában), keresési hibákat kaphat, például a CS008-009 és a CS012-002.</span><span class="sxs-lookup"><span data-stu-id="f0e23-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="f0e23-110">Ebben az esetben próbálkozzon újra a kereséssel a sikertelenül megjelenő tartalmi helyeken.</span><span class="sxs-lookup"><span data-stu-id="f0e23-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="f0e23-111">További információt  [ebben a cikkben](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) talál.</span><span class="sxs-lookup"><span data-stu-id="f0e23-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
