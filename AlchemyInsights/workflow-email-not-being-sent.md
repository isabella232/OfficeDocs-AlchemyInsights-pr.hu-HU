---
title: A munkafolyamat-e-mailek küldése nem történik meg
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748991"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="6578a-102">SharePoint-lista vagy-tár esetén a program nem küldi el a munkafolyamat-e-maileket</span><span class="sxs-lookup"><span data-stu-id="6578a-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="6578a-103">A munkafolyamatokból származó e-maileket a program nem küldi el az összes felhasználónak vagy csak bizonyos felhasználóknak, vagy ha a hibaüzenet az, hogy az e-mail **nem küldhető el. Győződjön meg arról, hogy az e-mailhez érvényes címzett tartozik**</span><span class="sxs-lookup"><span data-stu-id="6578a-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="6578a-104">Ellenőrizze, hogy a felhasználó megtalálható-e a webhelycsoporthoz tartozó **minden személy** engedélyei csoportban (felhasználói adatok listája).</span><span class="sxs-lookup"><span data-stu-id="6578a-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="6578a-105">Minta közvetlen URL: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="6578a-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="6578a-106">Ha a felhasználó nem létezik, győződjön meg arról, hogy a felhasználó be van jelentkezve a lapra.</span><span class="sxs-lookup"><span data-stu-id="6578a-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="6578a-107">Külső felhasználó esetén győződjön meg arról, hogy a meghívót elfogadták.</span><span class="sxs-lookup"><span data-stu-id="6578a-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="6578a-108">Ha a felhasználó létezik az engedélyek csoportban, ellenőrizze, hogy helyes-e az e-mail cím.</span><span class="sxs-lookup"><span data-stu-id="6578a-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="6578a-109">Ha a felhasználók e-mail-címe nincs beállítva, akkor hozzon létre egy, az adott felhasználóra vonatkozó figyelmeztetést, amely az adott felhasználói fiók szinkronizálását a SharePoint felhasználói profiljaiból ebbe a webhelycsoporthoz irányítja.</span><span class="sxs-lookup"><span data-stu-id="6578a-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="6578a-110">A munkafolyamatokból származó e-maileket a program a webhelycsoport rendszergazdáinak küldi el, a többi felhasználó számára azonban nem, és nem olvassa fel a \*\* <span>https:</span>//URL/_vti_bin/Client.xvc.Sp.Utilities.Utility.sendEmail\*\*.</span><span class="sxs-lookup"><span data-stu-id="6578a-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="6578a-111">Lásd: [hozzáférés megtagadva, amikor e-mailt küld egy SharePoint-csoportnak](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="6578a-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="6578a-112">Ellenőrizze azt is, hogy a **korlátozott hozzáférésű felhasználói engedély zárolási módja** webhelycsoport-szolgáltatás nem aktív.</span><span class="sxs-lookup"><span data-stu-id="6578a-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="6578a-113">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="6578a-113">Related topics</span></span>
<span data-ttu-id="6578a-114">Szeretné kipróbálni a Microsoft flow-t a SharePoint Online-ban?</span><span class="sxs-lookup"><span data-stu-id="6578a-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="6578a-115">Folyamatábra létrehozása</span><span class="sxs-lookup"><span data-stu-id="6578a-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="6578a-116">SharePoint és flow</span><span class="sxs-lookup"><span data-stu-id="6578a-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


