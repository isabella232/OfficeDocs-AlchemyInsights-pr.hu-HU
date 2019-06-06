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
ms.openlocfilehash: 5613138e7613deb264a7ab2c966f8b9c4a24763d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736405"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="1a0a3-102">Csak olvasásra szóló karbantartási jelenik meg, amikor próbál használni a SharePoint- vagy OneDrive</span><span class="sxs-lookup"><span data-stu-id="1a0a3-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="1a0a3-103">Jelenhet meg egy írásvédett karbantartási üzenet megkísérelte a SharePoint-vagy OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1a0a3-103">Users may receive a Read-Only for Maintenance message when attempting to use SharePoint or OneDrive.</span></span>

<span data-ttu-id="1a0a3-104">Ellenőrizze, nincs-e [Message center](https://portal.office.com/adminportal/home#/MessageCenter)navigáljon a bérlő bekövetkező aktív karbantartás.</span><span class="sxs-lookup"><span data-stu-id="1a0a3-104">Check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="1a0a3-105">Végezetül ellenőrizze, akkor látogassa meg a[Egészségügyi szolgáltatás](https://portal.office.com/adminportal/home#/servicehealth) , amely felmerülhet tanácsadók/események ellenőrzése.</span><span class="sxs-lookup"><span data-stu-id="1a0a3-105">Finally, ensure you visit the[Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="1a0a3-106">Ha sem az üzenet vagy szolgáltatás egészségügyi irányítópult tudomásul vették, aktuális karbantartási semmit a bérlő számára, ez lehet a böngésző gyorsítótár-probléma.</span><span class="sxs-lookup"><span data-stu-id="1a0a3-106">If neither the Message Center or Service Health Dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="1a0a3-107">Meg kell kísérelni a böngésző gyorsítótár kiürítése előtt nyissa meg a webhelyet.</span><span class="sxs-lookup"><span data-stu-id="1a0a3-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

- <span data-ttu-id="1a0a3-108">A Microsoft Edge böngészőben nyissa meg a további beállítások</span><span class="sxs-lookup"><span data-stu-id="1a0a3-108">In the Microsoft Edge browser, go to More  Settings</span></span>

- <span data-ttu-id="1a0a3-109">Egyértelmű böngészés kiválasztása válassza ki milyen jelet.</span><span class="sxs-lookup"><span data-stu-id="1a0a3-109">Under Clear browsing, select Choose what to clear.</span></span>
- <span data-ttu-id="1a0a3-110">Válassza ki a cookie-k és a webhely mentett adatok jelölőnégyzetet, és válassza ki a tiszta.</span><span class="sxs-lookup"><span data-stu-id="1a0a3-110">Select the Cookies and saved website data check box and select Clear.</span></span>

<span data-ttu-id="1a0a3-111">**Megjegyzés**: ezeket a lépéseket más böngészőkben, például a Firefox vagy Chrome használata esetén eltérő lehet.</span><span class="sxs-lookup"><span data-stu-id="1a0a3-111">**Note**: These steps may differ when using other browsers such as Firefox or Chrome.</span></span>

