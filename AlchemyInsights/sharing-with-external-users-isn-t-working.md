---
title: A külső felhasználókkal való megosztás nem működik
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502233"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="2dcab-102">A SharePoint-tartalom külső felhasználókkal való megosztását szolgáló problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="2dcab-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="2dcab-103">Győződjön meg arról, hogy a szervezeten belül be van kapcsolva a külső megosztás:</span><span class="sxs-lookup"><span data-stu-id="2dcab-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="2dcab-104">Keresse fel a [Microsoft &amp; 365 felügyeleti központ szolgáltatások bővítmények lapját](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), és kattintson a **helyek**gombra.</span><span class="sxs-lookup"><span data-stu-id="2dcab-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="2dcab-105">Ellenőrizze, hogy a beállítás be van-e kapcsolva.</span><span class="sxs-lookup"><span data-stu-id="2dcab-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="2dcab-106">Ha a "csak meglévő külső felhasználók" beállítás van kijelölve, ellenőrizze, hogy a külső felhasználó szerepel-e a Microsoft 365 felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="2dcab-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="2dcab-107">Ellenőrizze, hogy be van-e kapcsolva a webhely külső megosztása.</span><span class="sxs-lookup"><span data-stu-id="2dcab-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="2dcab-108">Részére egy klasszikus telek gyűjtemény:</span><span class="sxs-lookup"><span data-stu-id="2dcab-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="2dcab-109">Az új SharePoint admin központban kattintson a bal oldali ablaktáblán a **helyek**elemre.</span><span class="sxs-lookup"><span data-stu-id="2dcab-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="2dcab-110">Jelölje ki a webhelyet vagy webhelyeket, majd a szalagon kattintson a **megosztás**elemre.</span><span class="sxs-lookup"><span data-stu-id="2dcab-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="2dcab-111">Office 365-csoporthoz vagy kommunikációs webhelyhez tartozó csoportwebhely esetén:</span><span class="sxs-lookup"><span data-stu-id="2dcab-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="2dcab-112">Az új webhelytípusokhoz ugyanaz a megosztási beállítás van, mint a szervezeti szinten, kivéve, ha az egész szervezetre vonatkozó beállítás lehetővé teszi fájlok megosztását olyan hivatkozások segítségével, amelyekhez nem szükséges bejelentkezés.</span><span class="sxs-lookup"><span data-stu-id="2dcab-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="2dcab-113">Ebben az esetben a webhelyek lehetővé teszik a megosztást új és meglévő külső felhasználókkal, akik bejelentkeznek.</span><span class="sxs-lookup"><span data-stu-id="2dcab-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="2dcab-114">Az adott helyek beállításának megváltoztatásához használja az új SharePoint admin központot vagy a PowerShell parancshéjat.</span><span class="sxs-lookup"><span data-stu-id="2dcab-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="2dcab-115">[További információ](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="2dcab-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="2dcab-116">Az egyes webhelyek külső megosztási beállításai korlátozóbbak lehetnek, mint a szervezet egészére kiterjedő beállítások, de a szervezet egészére érvényes beállítás esetében nem megengedőbb.</span><span class="sxs-lookup"><span data-stu-id="2dcab-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

