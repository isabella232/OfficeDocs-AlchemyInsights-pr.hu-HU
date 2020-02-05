---
title: SharePoint-webhely létrehozása
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770857"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="9cb66-102">SharePoint-webhely létrehozása</span><span class="sxs-lookup"><span data-stu-id="9cb66-102">Create a SharePoint site</span></span>

<span data-ttu-id="9cb66-103">Webhelyek létrehozása vagy kezelése [az Aktív webhelyek](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) ből a SharePoint Felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="9cb66-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="9cb66-104">További információt [a Webhelyek kezelése az új SharePoint Felügyeleti központban](https://docs.microsoft.com/sharepoint/manage-site-creation)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="9cb66-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="9cb66-105">Tippek:</span><span class="sxs-lookup"><span data-stu-id="9cb66-105">Tips:</span></span>

- <span data-ttu-id="9cb66-106">**Nem** hozhat létre olyan webhelyet, amelynek URL-címe megegyezik egy meglévő webhely URL-címével.</span><span class="sxs-lookup"><span data-stu-id="9cb66-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="9cb66-107">Ha törölt egy webhelyet, és újra használni szeretné az URL-t, lehetséges, hogy a törölt webhely továbbra is létezik a [Törölt webhelyek](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)területen.</span><span class="sxs-lookup"><span data-stu-id="9cb66-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="9cb66-108">Az URL újbóli használatához a webhelyet véglegesen törölni kell.</span><span class="sxs-lookup"><span data-stu-id="9cb66-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="9cb66-109">Ha teljesen el szeretne távolítani egy webhelyet a Powershell használatával, olvassa el az [Eltávolítás spsite-parancsmag](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) példáját.</span><span class="sxs-lookup"><span data-stu-id="9cb66-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="9cb66-110">Előfordulhat, hogy egyes felhasználók nem tudnak webhelyet létrehozni.</span><span class="sxs-lookup"><span data-stu-id="9cb66-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="9cb66-111">[Lásd: Webhelylétrehozása kezelése a SharePoint Online-ban](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="9cb66-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="9cb66-112">Lehetséges, hogy a webhely a vártnál hosszabb ideig jelenik meg a **Létrehozás** oldalon.</span><span class="sxs-lookup"><span data-stu-id="9cb66-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="9cb66-113">Ha több mint 24 óra telt el azóta, hogy először látta ezt a problémát, kérjük, jelentkezzen be egy támogatási jegyet.</span><span class="sxs-lookup"><span data-stu-id="9cb66-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="9cb66-114">Sok esetben már dolgozunk a megoldáson.</span><span class="sxs-lookup"><span data-stu-id="9cb66-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="9cb66-115">Kérjük, adjon nekünk legalább 24 órát a megoldás befejezéséhez.</span><span class="sxs-lookup"><span data-stu-id="9cb66-115">Please give us at least 24 hours to complete a solution.</span></span>
