---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776084"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="55936-102">Tartalom keresés nem a várt eredmények visszaadása</span><span class="sxs-lookup"><span data-stu-id="55936-102">Content Search not returning expected results</span></span>

<span data-ttu-id="55936-103">Tartalom keresése az Office 365 biztonsági & Megfelelési központba történő futtatásakor váratlan keresési eredményeket kaphat.</span><span class="sxs-lookup"><span data-stu-id="55936-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="55936-104">Vegye figyelembe, amelyek hatással lehetnek a keresési eredmények a következők:</span><span class="sxs-lookup"><span data-stu-id="55936-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="55936-105">**Tartalom helye és a keresési feltételek**: Ellenőrizze, hogy a megfelelő tartalom helyének kiválasztott keresési feltételek.</span><span class="sxs-lookup"><span data-stu-id="55936-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="55936-106">Ha futtatta a nagy keresés (a számos helyen), érdemes több megkeresi azokat a darabolás.</span><span class="sxs-lookup"><span data-stu-id="55936-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="55936-107">**Részben indexelt elem**: a becsült keresési eredmények [részben indexelt elem](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) a postafiókok szerepelnek.</span><span class="sxs-lookup"><span data-stu-id="55936-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="55936-108">Azonban a OneDrive és a SharePoint-webhelyekről történő részleges indexelt elem nem szerepelnek a keresési becslés.</span><span class="sxs-lookup"><span data-stu-id="55936-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="55936-109">**Sikertelen keresés**: nagyszámú postafiókot (több mint 100 000 postafiókok) keresésekor jelenhet meg keresési hibák, a hibakódok CS008-009 és CS012-002).</span><span class="sxs-lookup"><span data-stu-id="55936-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="55936-110">Ebben az esetben próbálja meg újra a keresés csak a sikertelen tartalom helye.</span><span class="sxs-lookup"><span data-stu-id="55936-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="55936-111">[Ez a cikk](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) további információt talál.</span><span class="sxs-lookup"><span data-stu-id="55936-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
