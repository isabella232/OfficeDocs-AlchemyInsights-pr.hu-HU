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
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964881"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="7018a-102">Tartalom keresés nem a várt eredmények visszaadása</span><span class="sxs-lookup"><span data-stu-id="7018a-102">Content Search not returning expected results</span></span>

<span data-ttu-id="7018a-p101">Tartalom keresése az Office 365 biztonsági & Megfelelési központba történő futtatásakor váratlan keresési eredményeket kaphat. Vegye figyelembe, amelyek hatással lehetnek a keresési eredmények a következők:</span><span class="sxs-lookup"><span data-stu-id="7018a-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="7018a-p102">**Tartalom helye és a keresési feltételek**: Ellenőrizze, hogy a megfelelő tartalom helyének kiválasztott keresési feltételek. Ha futtatta a nagy keresés (a számos helyen), érdemes több megkeresi azokat a darabolás.</span><span class="sxs-lookup"><span data-stu-id="7018a-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="7018a-p103">**Részben indexelt elem**: a becsült keresési eredmények [részben indexelt elem](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) a postafiókok szerepelnek. Azonban a OneDrive és a SharePoint-webhelyekről történő részleges indexelt elem nem szerepelnek a keresési becslés.</span><span class="sxs-lookup"><span data-stu-id="7018a-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="7018a-p104">**Sikertelen keresés**: nagyszámú postafiókot (több mint 100 000 postafiókok) keresésekor jelenhet meg keresési hibák, a hibakódok CS008-009 és CS012-002). Ebben az esetben próbálja meg újra a keresés csak a sikertelen tartalom helye. [Ez a cikk](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) további információt talál.</span><span class="sxs-lookup"><span data-stu-id="7018a-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
