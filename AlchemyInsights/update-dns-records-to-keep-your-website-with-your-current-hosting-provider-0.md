---
title: A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi tárhelyszolgáltatónál
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665762"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="1846d-102">A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi tárhelyszolgáltatónál</span><span class="sxs-lookup"><span data-stu-id="1846d-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="1846d-103">A Microsoft 365 Felügyeleti központban nyissa meg a **Tartományok beállítása**  >  [Domains](https://portal.office.com/adminportal/home#/Domains) lapot, és a tartományok listájában válassza ki a webhelyhez használt tartományt.</span><span class="sxs-lookup"><span data-stu-id="1846d-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="1846d-104">Válassza az **+ Új egyéni rekord** elemet, és írja be az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="1846d-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="1846d-105">A **DNS típusa** mezőbe írja be az **A (Address)** értéket.</span><span class="sxs-lookup"><span data-stu-id="1846d-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="1846d-106">Az **Állomásnév vagy alias** mezőbe írja be a **@** karaktert.</span><span class="sxs-lookup"><span data-stu-id="1846d-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="1846d-107">Az **IP-cím** mezőbe írja be a statikus IP-címet, ahol a webhelye jelenleg üzemel (például 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="1846d-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="1846d-p101">Ennek a webhely  *statikus*  , és nem  *dinamikus*  IP-címének kell lennie. Azt a helyet ellenőrizve, ahol a webhelye üzemel, győződjön meg arról, hogy beszerezhet statikus IP-címet a nyilvános webhelyéhez.</span><span class="sxs-lookup"><span data-stu-id="1846d-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="1846d-110">Válassza a **Mentés** elemet.</span><span class="sxs-lookup"><span data-stu-id="1846d-110">Select **Save**.</span></span>

<span data-ttu-id="1846d-111">Ezenkívül egy CNAME rekordot is létrehozhat, hogy az ügyfelek könnyebben megtalálják a webhelyet.</span><span class="sxs-lookup"><span data-stu-id="1846d-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="1846d-112">Válassza az **+ Új egyéni rekord** elemet, és írja be az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="1846d-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="1846d-113">A **DNS típusa** mezőbe írja be a **CNAME (Alias)** értéket.</span><span class="sxs-lookup"><span data-stu-id="1846d-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="1846d-114">Az **Állomásnév vagy alias** mezőbe írja be a **www** értéket.</span><span class="sxs-lookup"><span data-stu-id="1846d-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="1846d-115">A **Célcím** mezőbe írja be a webhely teljes tartománynevét (FQDN) (például: contoso.com).</span><span class="sxs-lookup"><span data-stu-id="1846d-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="1846d-116">Válassza a **Mentés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="1846d-116">Select **Save**.</span></span>
