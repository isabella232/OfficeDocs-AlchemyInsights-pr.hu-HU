---
title: Napi elektronikus levél korlátoz kimagaslik. A munkafolyamat felfüggesztve.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053119"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="aa3d9-103">Napi email limit túllépve.</span><span class="sxs-lookup"><span data-stu-id="aa3d9-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="aa3d9-104">A munkafolyamat felfüggesztve.</span><span class="sxs-lookup"><span data-stu-id="aa3d9-104">Workflow is suspended.</span></span>

<span data-ttu-id="aa3d9-105">A hiba a következő helyzetekben jelenhet meg:</span><span class="sxs-lookup"><span data-stu-id="aa3d9-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="aa3d9-106">Olyan munkafolyamatot használ a SharePoint Online szolgáltatásban, amely a SharePoint 2010 vagy SharePoint 2013 munkafolyamat-platformtípust használja.</span><span class="sxs-lookup"><span data-stu-id="aa3d9-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="aa3d9-107">A munkafolyamat úgy van beállítva, hogy egy egyéni e-mail üzenetet több mint 200 felhasználók részére küld egy időben, több mint 10 000 címzettek naponta, vagy több mint 30 üzenet percenként.</span><span class="sxs-lookup"><span data-stu-id="aa3d9-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="aa3d9-108">A munkafolyamat futtatásakor az e-mail üzenetet a rendszer nem küldi el, és a következő viselkedést észleli:</span><span class="sxs-lookup"><span data-stu-id="aa3d9-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="aa3d9-109">A SharePoint 2013 platformtípust használó munkafolyamat esetén tallózással keresse meg a **munkafolyamat állapota** lapot.</span><span class="sxs-lookup"><span data-stu-id="aa3d9-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="aa3d9-110">A Munkafolyamat állapota lapon a **belső állapot** beállítása **elindítva**, az információs buborék pedig **nem tud elküldeni a címzettnek**.</span><span class="sxs-lookup"><span data-stu-id="aa3d9-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="aa3d9-111">A probléma kerülő megoldásához konfigurálja úgy a munkafolyamatot, hogy az e-mail üzeneteket az [Exchange Online küldőjéhez megadott korlátok](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)túllépése nélkül küldje el.</span><span class="sxs-lookup"><span data-stu-id="aa3d9-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="aa3d9-112">Például szüneteltetheti a munkafolyamatot a munkafolyamatban, elküldheti az e-mailt egy Office 365-csoportnak, terjesztési csoportnak vagy levelezési csoport számára engedélyezett biztonsági csoportnak, illetve elküldheti az üzenetet egyszerre kevesebb, mint 200 címzettnek.</span><span class="sxs-lookup"><span data-stu-id="aa3d9-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="aa3d9-113">További információt a következő [cikkben](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)találhat:</span><span class="sxs-lookup"><span data-stu-id="aa3d9-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="aa3d9-114">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="aa3d9-114">Related topics</span></span>
- [<span data-ttu-id="aa3d9-115">Átfolyás létrehozása</span><span class="sxs-lookup"><span data-stu-id="aa3d9-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="aa3d9-116">SharePoint-és adatfolyam</span><span class="sxs-lookup"><span data-stu-id="aa3d9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 