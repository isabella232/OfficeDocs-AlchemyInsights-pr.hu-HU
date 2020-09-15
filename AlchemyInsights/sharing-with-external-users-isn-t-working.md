---
title: Nem működött a külső felhasználókkal való megosztás
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691577"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="ea445-102">SharePoint-tartalmak külső felhasználókkal való megosztásával kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="ea445-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="ea445-103">Győződjön meg arról, hogy a külső megosztás be van kapcsolva a szervezetben:</span><span class="sxs-lookup"><span data-stu-id="ea445-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="ea445-104">Nyissa meg a [szolgáltatások &amp; bővítmények lapot a Microsoft 365 felügyeleti központban](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), és kattintson a **webhelyek**elemre.</span><span class="sxs-lookup"><span data-stu-id="ea445-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="ea445-105">Győződjön meg arról, hogy a beállítás be van kapcsolva.</span><span class="sxs-lookup"><span data-stu-id="ea445-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="ea445-106">Ha a "csak a meglévő külső felhasználók" beállítás van kiválasztva, győződjön meg arról, hogy a külső felhasználó szerepel a Microsoft 365 felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="ea445-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="ea445-107">Ellenőrizze, hogy be van-e kapcsolva a külső megosztás a webhelyen.</span><span class="sxs-lookup"><span data-stu-id="ea445-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="ea445-108">Klasszikus webhelycsoport esetén:</span><span class="sxs-lookup"><span data-stu-id="ea445-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="ea445-109">Az új SharePoint felügyeleti központ bal oldali ablaktábláján kattintson a **webhelyek**elemre.</span><span class="sxs-lookup"><span data-stu-id="ea445-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="ea445-110">Jelölje ki a webhelyet vagy a webhelyeket, és kattintson a menüszalag **megosztás**gombjára.</span><span class="sxs-lookup"><span data-stu-id="ea445-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="ea445-111">Microsoft 365-csoportba tartozó csoportwebhely vagy kommunikációs webhely esetén:</span><span class="sxs-lookup"><span data-stu-id="ea445-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="ea445-112">Ezek az új tartalomtípusok ugyanazzal a megosztási beállítással rendelkeznek, mint a szervezeti szintű beállítás, kivéve ha a szervezeti szintű beállítás lehetővé teszi a fájlok megosztását a bejelentkezést nem igénylő hivatkozásokkal.</span><span class="sxs-lookup"><span data-stu-id="ea445-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="ea445-113">Ebben az esetben a webhelyek lehetővé teszik a megosztást az új és a meglévő külső felhasználókkal, akik bejelentkeznek.</span><span class="sxs-lookup"><span data-stu-id="ea445-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="ea445-114">Ha módosítani szeretné bizonyos webhelyek beállítását, használja az új SharePoint felügyeleti központot vagy a PowerShellt.</span><span class="sxs-lookup"><span data-stu-id="ea445-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="ea445-115">[További információ](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="ea445-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="ea445-116">A webhelyek külső megosztási beállítása több korlátozást tartalmazhat, mint a szervezeti szintű beállítás, de nem több megengedhető érték, mint a szervezeti szintű beállítás.</span><span class="sxs-lookup"><span data-stu-id="ea445-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

