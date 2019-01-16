---
title: A külső felhasználók megosztása nem működik
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293858"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="c83cf-102">A SharePoint-tartalom megosztása a külső felhasználók problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="c83cf-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="c83cf-103">Ellenőrizze, hogy a szervezet külső megosztás van kapcsolva:</span><span class="sxs-lookup"><span data-stu-id="c83cf-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="c83cf-104">Keresse fel a [szolgáltatások &amp; -bővítmények lap az Office 365 felügyeleti központban](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), majd a **helyek**gombra.</span><span class="sxs-lookup"><span data-stu-id="c83cf-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="c83cf-p101">Győződjön meg arról, hogy a beállítás be van kapcsolva, "On." Ha be van jelölve "Csak meglévő külső felhasználók", ellenőrizze, hogy a külső felhasználó szerepel az Office 365 felügyeleti központ.</span><span class="sxs-lookup"><span data-stu-id="c83cf-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="c83cf-p102">Ellenőrizze, hogy a webhely kapcsolva külső megosztás. Klasszikus helycsoport:</span><span class="sxs-lookup"><span data-stu-id="c83cf-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="c83cf-109">A klasszikus SharePoint felügyeleti központ bal oldali ablaktáblájában kattintson a **webhelycsoportok**.</span><span class="sxs-lookup"><span data-stu-id="c83cf-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="c83cf-110">Jelölje ki a hely vagy helyek, és a menüszalagon kattintson a **megosztás**parancsra.</span><span class="sxs-lookup"><span data-stu-id="c83cf-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="c83cf-111">Az Office 365 csoporthoz tartozó csoportwebhelyet, vagy kommunikációs hely:</span><span class="sxs-lookup"><span data-stu-id="c83cf-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="c83cf-p103">Új webhely típusaival rendelkezik az azonos megosztási beállítása a szervezeti szintű beállítás, kivéve, ha a szervezeti szintű beállítás lehetővé teszi, hogy nem szükséges bejelentkezési hivatkozásokra fájlok megosztása. Ebben az esetben a webhelyek új és meglévő külső felhasználók bejelentkezés megosztás engedélyezése. Az új SharePoint felügyeleti központ (kép) vagy a PowerShell segítségével bizonyos webhelyek módosításához. [Tudjon meg többet](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="c83cf-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="c83cf-116">A külső webhelyek megosztási beállítása lehet szigorúbb, mint a szervezeti szintű beállítást, de nem több mint a szervezeti szintű beállítás alkalmazásszolgáltatásokra.</span><span class="sxs-lookup"><span data-stu-id="c83cf-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

