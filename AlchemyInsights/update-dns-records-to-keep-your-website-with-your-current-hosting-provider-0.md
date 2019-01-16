---
title: A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi tárhelyszolgáltatónál
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293522"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="b404a-102">A DNS-rekordok frissítése, hogy a webhely megmaradjon a jelenlegi tárhelyszolgáltatónál</span><span class="sxs-lookup"><span data-stu-id="b404a-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="b404a-103">A [Tartományok](https://portal.office.com/adminportal/home#/Domains) lapon válassza ki a webhelyhez használandó tartományt a tartományok listájából, és válassza a **DNS-beállítások** lehetőséget a felügyeleti panelen.</span><span class="sxs-lookup"><span data-stu-id="b404a-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="b404a-104">Válassza az **+ Új egyéni rekord** elemet, és írja be az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="b404a-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="b404a-105">A **DNS típusa** mezőbe írja be az **A (Address)** értéket.</span><span class="sxs-lookup"><span data-stu-id="b404a-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="b404a-106">Az **Állomásnév vagy alias** mezőbe írja be a **@** karaktert.</span><span class="sxs-lookup"><span data-stu-id="b404a-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="b404a-107">Az **IP-cím** mezőbe írja be a statikus IP-címet, ahol a webhelye jelenleg üzemel (például 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="b404a-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="b404a-p101">Ennek a webhely  *statikus*  , és nem  *dinamikus*  IP-címének kell lennie. Azt a helyet ellenőrizve, ahol a webhelye üzemel, győződjön meg arról, hogy beszerezhet statikus IP-címet a nyilvános webhelyéhez.</span><span class="sxs-lookup"><span data-stu-id="b404a-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="b404a-110">Válassza a **Mentés** elemet.</span><span class="sxs-lookup"><span data-stu-id="b404a-110">Select **Save**.</span></span> 
    
<span data-ttu-id="b404a-111">Ezenkívül egy CNAME rekordot is létrehozhat, hogy az ügyfelek könnyebben megtalálják a webhelyet.</span><span class="sxs-lookup"><span data-stu-id="b404a-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="b404a-112">Válassza az **+ Új egyéni rekord** elemet, és írja be az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="b404a-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="b404a-113">A **DNS típusa** mezőbe írja be a **CNAME (Alias)** értéket.</span><span class="sxs-lookup"><span data-stu-id="b404a-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="b404a-114">Az **Állomásnév vagy alias** mezőbe írja be a **www** értéket.</span><span class="sxs-lookup"><span data-stu-id="b404a-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="b404a-115">A **Célcím** mezőbe írja be a webhely teljes tartománynevét (FQDN) (például: contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b404a-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="b404a-116">Válassza a **Mentés** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="b404a-116">Select **Save**.</span></span> 
    

