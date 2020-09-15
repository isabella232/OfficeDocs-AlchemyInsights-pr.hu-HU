---
title: A SharePoint vagy a OneDrive használatakor a karbantartási üzenet írásvédett
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670834"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="89935-102">A SharePoint vagy a OneDrive használatakor a karbantartási üzenet írásvédett</span><span class="sxs-lookup"><span data-stu-id="89935-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="89935-103">A SharePoint vagy a OneDrive használatakor a felhasználók **csak olvashatóan kapják meg a karbantartási** üzenetet, ha a következő esetek egyikét kísérli meg használni.</span><span class="sxs-lookup"><span data-stu-id="89935-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="89935-104">Tervezett vagy aktív karbantartási tevékenység.</span><span class="sxs-lookup"><span data-stu-id="89935-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="89935-105">Ellenőrizze, hogy az [üzenetközpont](https://portal.office.com/adminportal/home#/messagecenter)segítségével navigáljon.</span><span class="sxs-lookup"><span data-stu-id="89935-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="89935-106">Nagy prioritású, aktív szolgáltatási incidens.</span><span class="sxs-lookup"><span data-stu-id="89935-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="89935-107">Ellenőrizze, hogy van-e valamilyen tanácsadója/incidense a [szolgáltatás állapotának](https://portal.office.com/adminportal/home#/servicehealth)megfelelő navigálásban.</span><span class="sxs-lookup"><span data-stu-id="89935-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="89935-108">Egy kisebb automatikus gyógyulási forgatókönyv, amely a kiszolgálók váratlan eseményei miatt az esetlegesen 30 percnél rövidebbek lehetnek.</span><span class="sxs-lookup"><span data-stu-id="89935-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="89935-109">Ezek a kisebb visszanyerések esetén nincsenek üzenetközpont vagy szolgáltatás-egészségügyi bejegyzések, de a szokásostól nagyon hamar vissza kell térnie.</span><span class="sxs-lookup"><span data-stu-id="89935-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="89935-110">Nagyon néhány esetben azt tapasztaltuk, hogy a fenti három eset egyike az oka, és a szolgáltatás vissza lett állítva, de a felhasználók böngésző-gyorsítótára nem törlődik.</span><span class="sxs-lookup"><span data-stu-id="89935-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="89935-111">A webhelyre való navigálás előtt próbálkozzon a gyorsítótár kiürítésével.</span><span class="sxs-lookup"><span data-stu-id="89935-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="89935-112">A Microsoft Edge böngészőben válassza a **Beállítások**, majd az **Adatvédelem és biztonság**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="89935-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="89935-113">A **böngészés törlése**csoportban válassza ki **a törölni kívánt**elemet.</span><span class="sxs-lookup"><span data-stu-id="89935-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="89935-114">Jelölje ki a **cookie-k és a mentett webhely adatai**lehetőséget, és válassza a **Törlés**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="89935-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="89935-115">Ezek a lépések eltérőek lehetnek más böngészők, például a Mozilla Firefox vagy a Google Chrome használatakor.</span><span class="sxs-lookup"><span data-stu-id="89935-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="89935-116">Egy másik lehetőség az, hogy megnyitja a SharePoint-webhelyet vagy a OneDrive egy új InPrivate-ablakban.</span><span class="sxs-lookup"><span data-stu-id="89935-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>