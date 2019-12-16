---
title: Írásvédett a karbantartási üzenet, amikor megpróbálja használni a SharePoint vagy a OneDrive
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051283"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="05c1d-102">Írásvédett a karbantartási üzenet, amikor megpróbálja használni a SharePoint vagy a OneDrive</span><span class="sxs-lookup"><span data-stu-id="05c1d-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="05c1d-103">A felhasználók a **karbantartási üzenetre csak olvasásra** kaphatnak értesítést, ha a következő forgatókönyvek valamelyikét próbálják használni a SharePoint vagy az OneDrive számára.</span><span class="sxs-lookup"><span data-stu-id="05c1d-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="05c1d-104">Tervezett vagy aktív karbantartási tevékenység.</span><span class="sxs-lookup"><span data-stu-id="05c1d-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="05c1d-105">Ellenőrizésükhöz navigáljon az [Üzenetközpontba](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="05c1d-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="05c1d-106">Az esetlegesen előforduló, magas prioritású, aktív szolgáltatási incidens.</span><span class="sxs-lookup"><span data-stu-id="05c1d-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="05c1d-107">Ellenőrizze az esetleges figyelmeztetéseket és eseményeket a navigáció a [szolgáltatás Health](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="05c1d-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="05c1d-108">A kisebb automatikus gyógyító hasznosítás forgatókönyv, hogy lehet történik, mivel minden váratlan események a szerverek, amelyek utolsó kevesebb, mint 30 perc, vagy úgy.</span><span class="sxs-lookup"><span data-stu-id="05c1d-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="05c1d-109">Nincs üzenet központ vagy szolgáltatás egészség póznák részére ezek kicsi behajtások de Önnek kellene lenni hát-hoz szabályos igazi nemsokára.</span><span class="sxs-lookup"><span data-stu-id="05c1d-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="05c1d-110">-Ra igazi kevés alkalom mi megfigyelt amit egyike három példák listázott fenti volt a okoz, és szolgáltatás van visszaad, de a használók legel elrejt ' ' tisztázódik.</span><span class="sxs-lookup"><span data-stu-id="05c1d-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="05c1d-111">Kérjük, mielőtt a webhelyre navigálnál, próbálja meg törölni a böngésző gyorsítótárát.</span><span class="sxs-lookup"><span data-stu-id="05c1d-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="05c1d-112">A Microsoft Edge böngészőben válassza a **Settings (beállítások**)-t, majd válassza a **Privacy és a Security**beállítást.</span><span class="sxs-lookup"><span data-stu-id="05c1d-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="05c1d-113">Alatt **tiszta szemöldök**, kiválaszt **választ mi-hoz tiszta**.</span><span class="sxs-lookup"><span data-stu-id="05c1d-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="05c1d-114">Válassza ki a **cookie-k és a mentett webhelyadatok**, majd a **Törlés**.</span><span class="sxs-lookup"><span data-stu-id="05c1d-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="05c1d-115">Ezek a lépések más böngészők, például a Mozilla Firefox vagy a Google Chrome használatakor eltérhetnek.</span><span class="sxs-lookup"><span data-stu-id="05c1d-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="05c1d-116">Másik választás akar lenni-hoz nyit-a SharePoint telek vagy OneDrive-ban egy új InPrivate ablak.</span><span class="sxs-lookup"><span data-stu-id="05c1d-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>