---
title: Csak olvasásra szóló karbantartási jelenik meg, amikor próbál használni a SharePoint- vagy OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620725"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="2c6b4-102">Csak olvasásra szóló karbantartási jelenik meg, amikor próbál használni a SharePoint- vagy OneDrive</span><span class="sxs-lookup"><span data-stu-id="2c6b4-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="2c6b4-103">Felhasználók is hibaüzenet **Írásvédett karbantartás** próbál használni a SharePoint- vagy OneDrive az alábbi esetek valamelyike.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="2c6b4-104">A tervezett és aktív karbantartási tevékenység.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="2c6b4-105">Ellenőrizze, hogy azokat a [Message Center](https://portal.office.com/adminportal/home#/messagecenter)navigáljon.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="2c6b4-106">Magas prioritású aktív szerviz esemény, amely felmerülhet.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="2c6b4-107">Ellenőrizze, hogy bármely tanácsadók eseményekre való [Egészségügyi szolgáltatás](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="2c6b4-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="2c6b4-108">Kisebb automatikus javító helyreállítás, a kiszolgálókon, amelyek kevesebb, mint 30 perc, vagy úgy lehet, hogy tart minden olyan váratlan események miatt sikerült előfordul.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="2c6b4-109">Vannak a nem Message Center vagy egészségügyi szolgáltatás által használt ezek kisebb helyreállítást de vissza a normál nagyon legrövidebb időn belül.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="2c6b4-110">Nagyon kevés alkalommal azt megfigyelhető, hogy a három fent említett esetek valamelyike okozhatta, és szolgáltatás visszaállította, de a felhasználók a böngésző gyorsítótár még nem lett bejelölve.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="2c6b4-111">Meg kell kísérelni a böngésző gyorsítótár kiürítése előtt nyissa meg a webhelyet.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="2c6b4-112">A Microsoft Edge böngészőben jelölje be a **Beállítások**, és válassza a **adatvédelmi és biztonsági**.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="2c6b4-113">**Egyértelmű böngészés**csoportban **Válassza ki, milyen jelet**.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="2c6b4-114">Jelölje be a **cookie-k és a mentett webhely adatokat**, és válassza a **világos**.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="2c6b4-115">Lépések eltérhetnek a más böngészőkben, például a Mozilla Firefox vagy Google Chrome használata során.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="2c6b4-116">Egy másik lehetőség az InPrivate-új ablakban nyílik meg a SharePoint-webhely vagy a OneDrive lenne.</span><span class="sxs-lookup"><span data-stu-id="2c6b4-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>