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
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840517"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="408c9-102">Csak olvasásra szóló karbantartási jelenik meg, amikor próbál használni a SharePoint- vagy OneDrive</span><span class="sxs-lookup"><span data-stu-id="408c9-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="408c9-103">Felhasználók is hibaüzenet **Írásvédett karbantartás** próbál használni a SharePoint- vagy OneDrive.</span><span class="sxs-lookup"><span data-stu-id="408c9-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive.</span></span>  <span data-ttu-id="408c9-104">Ha igen, ellenőrizze, nincs-e [Message center](https://portal.office.com/adminportal/home#/MessageCenter)navigáljon a bérlő bekövetkező aktív karbantartás.</span><span class="sxs-lookup"><span data-stu-id="408c9-104">If so, check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="408c9-105">Ellenőrizze, hogy az [Egészségügyi szolgáltatás](https://portal.office.com/adminportal/home#/servicehealth) irányítópult, amely felmerülhet tanácsadók/események ellenőrzése.</span><span class="sxs-lookup"><span data-stu-id="408c9-105">Also, make sure to check the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) dashboard to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="408c9-106">Ha sem az üzenet vagy egészségügyi szolgáltatás irányítópult tudomásul vették, aktuális karbantartási semmit a bérlő számára, ez lehet a böngésző gyorsítótár-probléma.</span><span class="sxs-lookup"><span data-stu-id="408c9-106">If neither the Message Center or Service Health dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="408c9-107">Meg kell kísérelni a böngésző gyorsítótár kiürítése előtt nyissa meg a webhelyet.</span><span class="sxs-lookup"><span data-stu-id="408c9-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="408c9-108">A Microsoft Edge böngészőben jelölje be a **Beállítások**, és válassza a **adatvédelmi és biztonsági**.</span><span class="sxs-lookup"><span data-stu-id="408c9-108">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="408c9-109">**Egyértelmű böngészés**csoportban **Válassza ki, milyen jelet**.</span><span class="sxs-lookup"><span data-stu-id="408c9-109">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="408c9-110">Jelölje be a **cookie-k és a mentett webhely adatokat**, és válassza a **világos**.</span><span class="sxs-lookup"><span data-stu-id="408c9-110">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="408c9-111">Lépések eltérhetnek a más böngészőkben, például a Mozilla Firefox vagy Google Chrome használata során.</span><span class="sxs-lookup"><span data-stu-id="408c9-111">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="408c9-112">Egy másik lehetőség az InPrivate-új ablakban nyílik meg a SharePoint-webhely vagy a OneDrive lenne.</span><span class="sxs-lookup"><span data-stu-id="408c9-112">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>