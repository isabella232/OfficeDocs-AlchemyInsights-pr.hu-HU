---
title: eDiscovery exportálási eszköze
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277924"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="ad82d-102">Nem lehet telepíteni vagy futtatni az eDiscovery exportálási eszközét?</span><span class="sxs-lookup"><span data-stu-id="ad82d-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="ad82d-103">Ha nem tudja telepíteni vagy futtatni az eDiscovery exportálási eszközét a keresési eredmények letöltéséhez, ellenőrizze az alábbi dolgokat:</span><span class="sxs-lookup"><span data-stu-id="ad82d-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="ad82d-104">A használt számítógép megfelel az alábbi előfeltételeknek:</span><span class="sxs-lookup"><span data-stu-id="ad82d-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="ad82d-105">a Windows 7 és a későbbi verziók 32-vagy 64-bites verziója</span><span class="sxs-lookup"><span data-stu-id="ad82d-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="ad82d-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="ad82d-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="ad82d-107">Támogatott böngésző:</span><span class="sxs-lookup"><span data-stu-id="ad82d-107">A supported browser:</span></span>

  - <span data-ttu-id="ad82d-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ad82d-108">Microsoft Edge</span></span>

    <span data-ttu-id="ad82d-109">Vagy</span><span class="sxs-lookup"><span data-stu-id="ad82d-109">Or</span></span>

  - <span data-ttu-id="ad82d-110">Internet Explorer 10 vagy újabb verziók</span><span class="sxs-lookup"><span data-stu-id="ad82d-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="ad82d-111">Más böngészők, mint például a Google Chrome és a Mozilla Firefox, nem támogatottak.</span><span class="sxs-lookup"><span data-stu-id="ad82d-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="ad82d-112">Szervezete elérheti a végpontot az Azure-ban, amely \*\* \* . blob.Core.Windows.net\*\* (a helyettesítő karakter az exportálási feladat egyedi azonosítóját jelenti).</span><span class="sxs-lookup"><span data-stu-id="ad82d-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="ad82d-113">Az exportálási szerepkört hozzárendelte a Microsoft 365 biztonsági &amp; megfelelőségi központban.</span><span class="sxs-lookup"><span data-stu-id="ad82d-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="ad82d-114">Alapértelmezés szerint ez a szerepkör csak az eDiscovery-kezelő szerepkörcsoport szerepkör-csoportjához van társítva.</span><span class="sxs-lookup"><span data-stu-id="ad82d-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="ad82d-115">Lásd: [eDiscovery-engedélyek hozzárendelése](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="ad82d-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="ad82d-116">További információt a tartalmi találatok [exportálása](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)című témakörben találhat.</span><span class="sxs-lookup"><span data-stu-id="ad82d-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="ad82d-117">Ha több, mint 100K postaládát exportál, a következő PowerShell-lel kell használnia az Exportálás eredményének letöltéséhez:  [eredmények exportálása több mint 100k postaládából](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="ad82d-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>