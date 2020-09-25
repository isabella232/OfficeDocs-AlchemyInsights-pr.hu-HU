---
title: 1490-hibaelhárítás-eDiscovery-hibák
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277833"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="5c0ff-102">Tartalmi keresési hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="5c0ff-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="5c0ff-103">Problémákat tapasztal a tartalmi kereséssel kapcsolatban, vagy problémákat tapasztal a keresési eredmények exportálásakor?</span><span class="sxs-lookup"><span data-stu-id="5c0ff-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="5c0ff-104">A keresések futtatásakor például a következőket kapja meg?</span><span class="sxs-lookup"><span data-stu-id="5c0ff-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="5c0ff-105">CS008 vagy CS012 hibák</span><span class="sxs-lookup"><span data-stu-id="5c0ff-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="5c0ff-106">A kiszolgáló foglalt/időtúllépési hibája</span><span class="sxs-lookup"><span data-stu-id="5c0ff-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="5c0ff-107">Alkalmazási hiba történt</span><span class="sxs-lookup"><span data-stu-id="5c0ff-107">Application error occurred</span></span>

<span data-ttu-id="5c0ff-108">Vagy ha nagy számú postaládából keres vagy exportál találatokat (több mint 100 000-postaládában), az exportálási hibákat kapja?</span><span class="sxs-lookup"><span data-stu-id="5c0ff-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="5c0ff-109">Az ilyen típusú hibák esetén próbálkozzon a sikertelenül megjelenő tartalmi helyek keresésével.</span><span class="sxs-lookup"><span data-stu-id="5c0ff-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="5c0ff-110">További információt  [ebben a cikkben](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) talál.</span><span class="sxs-lookup"><span data-stu-id="5c0ff-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="5c0ff-111">Ha több, mint 100K postaládát exportál, a következő PowerShell-lel kell használnia az Exportálás eredményének letöltéséhez:  [eredmények exportálása több mint 100k postaládából](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="5c0ff-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
