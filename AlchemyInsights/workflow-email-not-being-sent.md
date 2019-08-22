---
title: A munkafolyamat e-mailben nem küldi el
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530877"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="63953-102">A munkafolyamat e-mailben nem küldi a SharePoint-lista vagy tár</span><span class="sxs-lookup"><span data-stu-id="63953-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="63953-103">Munkafolyamatok e-mail az összes felhasználóra vagy csak bizonyos felhasználók nem kapnak, vagy megtekintheti a hiba **az e-mail üzenet nem küldhető el. Győződjön meg arról, hogy az e-mail rendelkezik-e érvényes címzettel**.</span><span class="sxs-lookup"><span data-stu-id="63953-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="63953-104">Ellenőrizze, hogy a felhasználó a **Mindenki** engedélyei csoport (felhasználói adatok listája) a webhelycsoport létezik.</span><span class="sxs-lookup"><span data-stu-id="63953-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="63953-105">Minta közvetlen URL-cím: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="63953-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="63953-106">Ha a felhasználó nem létezik, ellenőrizze, hogy a felhasználó a lapba van aláírva.</span><span class="sxs-lookup"><span data-stu-id="63953-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="63953-107">Ha egy külső felhasználó, győződjön meg arról, hogy a meghívást elfogadták.</span><span class="sxs-lookup"><span data-stu-id="63953-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="63953-108">Ha a felhasználó az engedélyek csoport létezik, ellenőrizze, hogy helyesek-e az e-mail címet.</span><span class="sxs-lookup"><span data-stu-id="63953-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="63953-109">Ha a felhasználó e-mail címe nincs megadva itt, hozzon létre egy mintát értesítés az adott felhasználó, amely arra kényszeríti a felhasználói fiók a szinkronizálás a SharePoint felhasználói profilok a webhelycsoportban.</span><span class="sxs-lookup"><span data-stu-id="63953-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="63953-110">A munkafolyamatok e-mail küld a helycsoport-rendszergazdák azonban nem mások, és hibaüzenet jelenik **HTTP tilos <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="63953-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="63953-111">Lásd: [Hozzáférés megtagadva, ha küld egy e-mailt egy SharePoint-csoporthoz](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="63953-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="63953-112">Azt is ellenőrizze, hogy a **korlátozott hozzáférésű felhasználói engedély zárolási mód** webhelycsoport-szolgáltatás nincs bekapcsolva.</span><span class="sxs-lookup"><span data-stu-id="63953-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="63953-113">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="63953-113">Related topics</span></span>
<span data-ttu-id="63953-114">Próbálkozzon a SharePoint Online Microsoft Flow szeretne?</span><span class="sxs-lookup"><span data-stu-id="63953-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="63953-115">Folyamat létrehozása</span><span class="sxs-lookup"><span data-stu-id="63953-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="63953-116">A SharePoint és az áram</span><span class="sxs-lookup"><span data-stu-id="63953-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


