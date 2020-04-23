---
title: Nem működik a megosztás külső felhasználókkal
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767251"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="cab7d-102">A SharePoint-tartalmak külső felhasználókkal való megosztásával kapcsolatos problémák megoldása</span><span class="sxs-lookup"><span data-stu-id="cab7d-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="cab7d-103">Győződjön meg arról, hogy a külső megosztás be van kapcsolva a szervezetnél:</span><span class="sxs-lookup"><span data-stu-id="cab7d-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="cab7d-104">Nyissa meg a [Microsoft 365 Felügyeleti központ &amp; Szolgáltatások bővítményeit tartalmazó lapot,](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)és kattintson a Webhelyek **gombra.**</span><span class="sxs-lookup"><span data-stu-id="cab7d-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="cab7d-105">Ellenőrizze, hogy a beállítás be van-e kapcsolva.</span><span class="sxs-lookup"><span data-stu-id="cab7d-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="cab7d-106">Ha a "Csak a meglévő külső felhasználók" jelölőnégyzet be van jelölve, ellenőrizze, hogy a külső felhasználó szerepel-e a Microsoft 365 Felügyeleti központban.</span><span class="sxs-lookup"><span data-stu-id="cab7d-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="cab7d-107">Győződjön meg arról, hogy a külső megosztás be van kapcsolva a webhelyen.</span><span class="sxs-lookup"><span data-stu-id="cab7d-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="cab7d-108">Klasszikus webhelycsoport esetén:</span><span class="sxs-lookup"><span data-stu-id="cab7d-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="cab7d-109">Az új SharePoint Felügyeleti központban, a bal oldali ablaktáblában kattintson a **Webhelyek**elemre.</span><span class="sxs-lookup"><span data-stu-id="cab7d-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="cab7d-110">Jelölje ki a webhelyet vagy webhelyeket, és a menüszalagon kattintson a **Megosztás gombra.**</span><span class="sxs-lookup"><span data-stu-id="cab7d-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="cab7d-111">Office 365-csoporthoz vagy kommunikációs webhelyhez tartozó csoportwebhely esetén:</span><span class="sxs-lookup"><span data-stu-id="cab7d-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="cab7d-112">Ezek az új webhelytípusok ugyanazt a megosztási beállítást, mint a szervezeti szintű beállítás, kivéve, ha a szervezeti szintű beállítás lehetővé teszi a fájlok megosztását olyan hivatkozások használatával, amelyek nem igényelnek bejelentkezést.</span><span class="sxs-lookup"><span data-stu-id="cab7d-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="cab7d-113">Ebben az esetben a webhelyek lehetővé teszik a megosztást a bejelentkező új és meglévő külső felhasználókkal.</span><span class="sxs-lookup"><span data-stu-id="cab7d-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="cab7d-114">Adott webhelyek beállításának módosításához használja az új SharePoint Felügyeleti központot vagy a PowerShellt.</span><span class="sxs-lookup"><span data-stu-id="cab7d-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="cab7d-115">[További információ](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="cab7d-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="cab7d-116">A külső megosztási beállítás bármely webhelyesetében szigorúbb lehet, mint a szervezeti szintű beállítás, de nem lehet megengedőbb, mint a szervezeti szintű beállítás.</span><span class="sxs-lookup"><span data-stu-id="cab7d-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

