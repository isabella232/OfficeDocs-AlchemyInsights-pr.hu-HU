---
title: A külső felhasználók megosztása nem működik
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502233"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="17c12-102">A SharePoint-tartalom megosztása a külső felhasználók problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="17c12-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="17c12-103">Ellenőrizze, hogy a szervezet külső megosztás van kapcsolva:</span><span class="sxs-lookup"><span data-stu-id="17c12-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="17c12-104">Keresse fel a [szolgáltatások &amp; -bővítmények a Microsoft 365 felügyeleti központ lapján](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), majd a **helyek**gombra.</span><span class="sxs-lookup"><span data-stu-id="17c12-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="17c12-105">Győződjön meg arról, hogy a beállítás be van kapcsolva, "On."</span><span class="sxs-lookup"><span data-stu-id="17c12-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="17c12-106">Ha be van jelölve "Csak meglévő külső felhasználók", ellenőrizze, hogy a külső felhasználói a Microsoft 365 felügyeleti központ szerepel.</span><span class="sxs-lookup"><span data-stu-id="17c12-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="17c12-107">Ellenőrizze, hogy a webhely kapcsolva külső megosztás.</span><span class="sxs-lookup"><span data-stu-id="17c12-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="17c12-108">Klasszikus helycsoport:</span><span class="sxs-lookup"><span data-stu-id="17c12-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="17c12-109">Az új SharePoint felügyeleti központ bal oldali ablaktáblájában kattintson a **helyek**gombra.</span><span class="sxs-lookup"><span data-stu-id="17c12-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="17c12-110">Jelölje ki a hely vagy helyek, és a menüszalagon kattintson a **megosztás**parancsra.</span><span class="sxs-lookup"><span data-stu-id="17c12-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="17c12-111">Az Office 365 csoporthoz tartozó csoportwebhelyet, vagy kommunikációs hely:</span><span class="sxs-lookup"><span data-stu-id="17c12-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="17c12-112">Új webhely típusaival rendelkezik az azonos megosztási beállítása a szervezeti szintű beállítás, kivéve, ha a szervezeti szintű beállítás lehetővé teszi, hogy nem szükséges bejelentkezési hivatkozásokra fájlok megosztása.</span><span class="sxs-lookup"><span data-stu-id="17c12-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="17c12-113">Ebben az esetben a webhelyek új és meglévő külső felhasználók bejelentkezés megosztás engedélyezése.</span><span class="sxs-lookup"><span data-stu-id="17c12-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="17c12-114">Bizonyos webhelyek módosításához használja az új SharePoint-felügyeleti központ vagy PowerShell.</span><span class="sxs-lookup"><span data-stu-id="17c12-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="17c12-115">[További információ](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="17c12-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="17c12-116">A külső webhelyek megosztási beállítása lehet szigorúbb, mint a szervezeti szintű beállítást, de nem több mint a szervezeti szintű beállítás alkalmazásszolgáltatásokra.</span><span class="sxs-lookup"><span data-stu-id="17c12-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

