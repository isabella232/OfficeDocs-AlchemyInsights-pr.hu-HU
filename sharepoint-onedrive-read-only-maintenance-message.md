---
title: E-mailben kap egy TenantAccessBlockedException hiba elérésekor 127?
ms.author: kirks
author: Techwriter40
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
ms.openlocfilehash: 54ebc269b391e6b0d607e55af8283ebf3d9e2aa7
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715074"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="1808e-102">Csak olvasásra szóló karbantartási jelenik meg, amikor próbál használni a SharePoint- vagy OneDrive</span><span class="sxs-lookup"><span data-stu-id="1808e-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="1808e-103">Jelenhet meg egy írásvédett karbantartási üzenet megkísérelte a SharePoint-vagy OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1808e-103">Users may receive a Read-Only for Maintenance message when attempting to use SharePoint or OneDrive.</span></span>

<span data-ttu-id="1808e-104">Ellenőrizze, nincs-e <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>navigáljon a bérlő bekövetkező aktív karbantartás.</span><span class="sxs-lookup"><span data-stu-id="1808e-104">Check if there is active maintenance occurring on your tenant by navigating to the <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>.</span></span> <span data-ttu-id="1808e-105">Végezetül ellenőrizze, akkor látogassa meg a <a href="https://portal.office.com/adminportal/home#/servicehealth">Egészségügyi szolgáltatás</a> , amely felmerülhet tanácsadók/események ellenőrzése.</span><span class="sxs-lookup"><span data-stu-id="1808e-105">Finally, ensure you visit the <a href="https://portal.office.com/adminportal/home#/servicehealth">Service Health</a> page to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="1808e-106">Ha sem az üzenet vagy szolgáltatás egészségügyi irányítópult tudomásul vették, aktuális karbantartási semmit a bérlő számára, ez lehet a böngésző gyorsítótár-probléma.</span><span class="sxs-lookup"><span data-stu-id="1808e-106">If neither the Message Center or Service Health Dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="1808e-107">Meg kell kísérelni a böngésző gyorsítótár kiürítése előtt nyissa meg a webhelyet.</span><span class="sxs-lookup"><span data-stu-id="1808e-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

  <li><span data-ttu-id="1808e-108">A Microsoft Edge böngészőben Ugrás <strong>több &hellip; &gt; beállítások</strong></span><span class="sxs-lookup"><span data-stu-id="1808e-108">In the Microsoft Edge browser, go to <strong>More &hellip;&gt; Settings</strong></span></span></li>  <li><span data-ttu-id="1808e-109"><strong>Egyértelmű böngészés </strong>csoportban <strong>Válassza ki, milyen jelet</strong>.</span><span class="sxs-lookup"><span data-stu-id="1808e-109">Under <strong>Clear browsing </strong>, select <strong>Choose what to clear</strong>.</span></span></li>  <li><span data-ttu-id="1808e-110">Válassza ki a cookie-k és a webhely mentett adatok jelölőnégyzetet, és válassza ki a <strong>törlése</strong>.</span><span class="sxs-lookup"><span data-stu-id="1808e-110">Select the Cookies and saved website data check box and select <strong>Clear</strong>.</span></span></li>  </ol>  

<span data-ttu-id="1808e-111">**Megjegyzés**: ezeket a lépéseket más böngészőkben, például a Firefox vagy Chrome használata esetén eltérő lehet.</span><span class="sxs-lookup"><span data-stu-id="1808e-111">**Note**: These steps may differ when using other browsers such as Firefox or Chrome.</span></span>

