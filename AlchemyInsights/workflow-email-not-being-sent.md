---
title: A munkafolyamat-e-mail nem kerül elküldésre
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049375"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="20c40-102">A munkafolyamat-e-mail nem lett elküldve SharePoint-listához vagy-tárhoz</span><span class="sxs-lookup"><span data-stu-id="20c40-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="20c40-103">A munkafolyamatokból származó e-maileket nem küldi el a rendszer az összes felhasználónak vagy csak bizonyos felhasználóknak, vagy az **e-mail üzenetet nem lehet elküldeni. Győződj meg a elektronikus levél birtokol egy érvényes fogékony**.</span><span class="sxs-lookup"><span data-stu-id="20c40-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="20c40-104">Ellenőrizze, hogy a felhasználó szerepel-e az adott webhelycsoport **minden személy** engedélyei csoportjában (felhasználói adatok listájában).</span><span class="sxs-lookup"><span data-stu-id="20c40-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="20c40-105">Minta közvetlen URL: https://<tenant>. sharepoint.com/sites/<sitename>/_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="20c40-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="20c40-106">Ha a felhasználó nem létezik, győződjön meg arról, hogy a felhasználó be van jelentkezve az oldalra.</span><span class="sxs-lookup"><span data-stu-id="20c40-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="20c40-107">Ha külső felhasználó, akkor győződjön meg arról, hogy meghívásukat elfogadták.</span><span class="sxs-lookup"><span data-stu-id="20c40-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="20c40-108">Ha a felhasználó az engedélycsoportban is szerepel, ellenőrizze, hogy az e-mail cím helyes-e.</span><span class="sxs-lookup"><span data-stu-id="20c40-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="20c40-109">Ha a felhasználók e-mail címe nincs beállítva, akkor hozzon létre egy mintafigyelmeztetést arra a felhasználóra vonatkozóan, amely az adott felhasználói fióknak a SharePoint felhasználói profiljaihoz való szinkronizálását kényszeríti erre a webhelygyűjteményre.</span><span class="sxs-lookup"><span data-stu-id="20c40-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="20c40-110">A munkafolyamatokból érkező e-maileket a rendszer a webhelycsoport rendszergazdáinak küldi, de a többi felhasználónak nem, és a **http tiltott és <span>https:</span>//URL/_vti_bin/Client.xvc.Sp.Utilities.Utility.sendEmail**hibát látja.</span><span class="sxs-lookup"><span data-stu-id="20c40-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="20c40-111">[Ha egy SharePoint-csoportnak küld e-mailt, tekintse át a hozzáférés megtagadva](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)választógombot.</span><span class="sxs-lookup"><span data-stu-id="20c40-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="20c40-112">Ellenőrizze azt is, hogy a **korlátozott hozzáférésű felhasználói engedély zárolási módja** helycsoport-szolgáltatás nem aktív-e.</span><span class="sxs-lookup"><span data-stu-id="20c40-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="20c40-113">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="20c40-113">Related topics</span></span>
<span data-ttu-id="20c40-114">Szeretné kipróbálni a Microsoft flow-t a SharePoint Online szolgáltatásban?</span><span class="sxs-lookup"><span data-stu-id="20c40-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="20c40-115">Átfolyás létrehozása</span><span class="sxs-lookup"><span data-stu-id="20c40-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="20c40-116">SharePoint-és adatfolyam</span><span class="sxs-lookup"><span data-stu-id="20c40-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


