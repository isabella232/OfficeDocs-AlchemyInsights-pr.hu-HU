---
title: Webhely végleges törlése a SharePointban
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955168"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="a8f15-102">Webhely végleges törlése a SharePointban</span><span class="sxs-lookup"><span data-stu-id="a8f15-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="a8f15-103">Ha újra fel szeretne használni egy URL-t egy törölt webhelyről (a webhely újbóli létrehozásához), vagy véglegesen törölni szeretné a webhelyet, mert az már nincs használatban, akkor használja az új SharePoint felügyeleti központból a **Végleges törlés** opciót.</span><span class="sxs-lookup"><span data-stu-id="a8f15-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="a8f15-104">Nyissa meg az [Új SharePoint felügyeleti központ törölt helyek lapját](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) és jelentkezzen be egy olyan fiókkal, amely rendszergazdai engedélyekkel rendelkezik a szervezetéhez.</span><span class="sxs-lookup"><span data-stu-id="a8f15-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="a8f15-105">A bal oldali oszlopban válasszon ki egy webhelyet.</span><span class="sxs-lookup"><span data-stu-id="a8f15-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="a8f15-106">Kattintson a **Végleges törlés**elemre.</span><span class="sxs-lookup"><span data-stu-id="a8f15-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="a8f15-107">**Megjegyzés**: a csoportosított webhely nem törölhető véglegesen az új SharePoint felügyeleti központból.</span><span class="sxs-lookup"><span data-stu-id="a8f15-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="a8f15-108">Ehelyett a [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) használata szükséges.</span><span class="sxs-lookup"><span data-stu-id="a8f15-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="a8f15-109">További információt a [Webhely végleges törlése](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site) témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="a8f15-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
