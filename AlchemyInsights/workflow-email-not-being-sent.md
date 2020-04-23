---
title: A munkafolyamat-e-mail küldése nem történik meg
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766135"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="d3674-102">A munkafolyamat-alapú e-mail nem küldő SharePoint-listához vagy tárhoz</span><span class="sxs-lookup"><span data-stu-id="d3674-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="d3674-103">A munkafolyamatokból származó e-mail eket a rendszer nem küldi el minden felhasználónak, vagy csak egy adott felhasználónak, vagy a hibaüzenet jelenik **meg: Az e-mail nem küldhető el. Győződjön meg arról, hogy az e-mailnek érvényes címzettje van.**</span><span class="sxs-lookup"><span data-stu-id="d3674-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="d3674-104">Ellenőrizze, hogy a felhasználó létezik-e az adott webhelycsoport **Minden személyek** engedélycsoportjában (felhasználói adatok listájában).</span><span class="sxs-lookup"><span data-stu-id="d3674-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="d3674-105">Minta közvetlen<tenant>URL:https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? Tagsági csoportazonosító=0</span><span class="sxs-lookup"><span data-stu-id="d3674-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="d3674-106">Ha a felhasználó nem létezik, ellenőrizze, hogy a felhasználó be van-e jelentkezve a lapra.</span><span class="sxs-lookup"><span data-stu-id="d3674-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="d3674-107">Ha külső felhasználóról van szó, győződjön meg arról, hogy a meghívást elfogadták.</span><span class="sxs-lookup"><span data-stu-id="d3674-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="d3674-108">Ha a felhasználó létezik az engedélycsoportban, ellenőrizze, hogy az e-mail cím helyes-e.</span><span class="sxs-lookup"><span data-stu-id="d3674-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="d3674-109">Ha a felhasználók e-mail címe nincs beállítva itt, akkor hozzon létre egy mintariasztást az adott felhasználó számára, amely kényszeríti az adott felhasználói fiók szinkronizálását a SharePoint felhasználói profiljaiból erre a webhelycsoportra.</span><span class="sxs-lookup"><span data-stu-id="d3674-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="d3674-110">A munkafolyamatokból származó e-maileket a rendszer elküldi a webhelycsoport rendszergazdáinak, de más felhasználóknak nem, és a HTTP Tiltott https hibát \*\* <span>látja:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail\*\*.</span><span class="sxs-lookup"><span data-stu-id="d3674-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="d3674-111">Lásd: [Hozzáférés megtagadva, ha e-mailt küld egy SharePoint-csoportnak.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)</span><span class="sxs-lookup"><span data-stu-id="d3674-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="d3674-112">Ellenőrizze azt is, hogy a **korlátozott hozzáférésű felhasználói engedélyek zárolási módú** webhelycsoport szolgáltatása nem aktív-e.</span><span class="sxs-lookup"><span data-stu-id="d3674-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="d3674-113">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="d3674-113">Related topics</span></span>
<span data-ttu-id="d3674-114">Kiszeretné próbálni a Microsoft Flow-t a SharePoint Online-ban?</span><span class="sxs-lookup"><span data-stu-id="d3674-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="d3674-115">Folyamat létrehozása</span><span class="sxs-lookup"><span data-stu-id="d3674-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d3674-116">SharePoint és Folyamat</span><span class="sxs-lookup"><span data-stu-id="d3674-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


