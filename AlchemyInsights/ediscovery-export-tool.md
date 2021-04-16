---
title: eDiscovery export tool
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814590"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="a3fa4-102">Nem tudja telepíteni vagy futtatni az Elektronikus adatok exportálása eszközt?</span><span class="sxs-lookup"><span data-stu-id="a3fa4-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="a3fa4-103">Ha nem tudja telepíteni vagy futtatni az Elektronikus adatok exportálása eszközt a keresési eredmények letöltéséhez, ellenőrizze az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="a3fa4-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="a3fa4-104">A használt számítógép megfelel az alábbi előfeltételeknek:</span><span class="sxs-lookup"><span data-stu-id="a3fa4-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="a3fa4-105">A Windows 7 és az újabb verziók 32 vagy 64 bites verziója</span><span class="sxs-lookup"><span data-stu-id="a3fa4-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="a3fa4-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="a3fa4-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="a3fa4-107">Támogatott böngésző:</span><span class="sxs-lookup"><span data-stu-id="a3fa4-107">A supported browser:</span></span>

  - <span data-ttu-id="a3fa4-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a3fa4-108">Microsoft Edge</span></span>

    <span data-ttu-id="a3fa4-109">Vagy</span><span class="sxs-lookup"><span data-stu-id="a3fa4-109">Or</span></span>

  - <span data-ttu-id="a3fa4-110">Internet Explorer 10 vagy újabb verziók</span><span class="sxs-lookup"><span data-stu-id="a3fa4-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="a3fa4-111">Más böngészők, például a Google Chrome és a Mozilla Firefox nem támogatottak.</span><span class="sxs-lookup"><span data-stu-id="a3fa4-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="a3fa4-112">Szervezete csatlakozhat az Azure-beli végponthoz, amely **\* .blob.core.windows.net** (a helyettesítő karakter az exportálási feladat egyedi azonosítóját jelöli).</span><span class="sxs-lookup"><span data-stu-id="a3fa4-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="a3fa4-113">Exportálási szerepkört kap a Microsoft 365 Biztonsági megfelelőségi &amp; központban.</span><span class="sxs-lookup"><span data-stu-id="a3fa4-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="a3fa4-114">Ez a szerepkör alapértelmezés szerint csak az Elektronikus észlelés-kezelő szerepkörcsoporthoz van hozzárendelve.</span><span class="sxs-lookup"><span data-stu-id="a3fa4-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="a3fa4-115">Lásd: [Elektronikus észlelési engedélyek hozzárendelése.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="a3fa4-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="a3fa4-116">További információ: [Tartalomkeresés eredményeinek exportálása.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="a3fa4-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="a3fa4-117">Ha több mint 100 000 000 postaládát exportál, a következő Powershell használatával kell letöltenie az Eredmények exportálása: Találatok exportálása több mint  [100 000 postaládából](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)parancsot.</span><span class="sxs-lookup"><span data-stu-id="a3fa4-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>