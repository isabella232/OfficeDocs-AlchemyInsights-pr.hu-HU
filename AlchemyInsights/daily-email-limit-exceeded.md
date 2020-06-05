---
title: A napi e-mail korlát túllépve. A munkafolyamat fel van függesztve.
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
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580335"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="faccd-103">Napi e-mail korlát túllépve.</span><span class="sxs-lookup"><span data-stu-id="faccd-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="faccd-104">A munkafolyamat fel van függesztve.</span><span class="sxs-lookup"><span data-stu-id="faccd-104">Workflow is suspended.</span></span>

<span data-ttu-id="faccd-105">Ez a hiba a következő esetekben jelenhet meg:</span><span class="sxs-lookup"><span data-stu-id="faccd-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="faccd-106">A SharePoint 2010 vagy a SharePoint 2013 munkafolyamat-platformtípusát használó SharePoint Online-munkafolyamattal rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="faccd-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="faccd-107">A munkafolyamat úgy van beállítva, hogy egyszerre több mint 200 felhasználónak, naponta több mint 10 000 címzettnek vagy percenként több mint 30 üzenetnek küldjön üzenetet.</span><span class="sxs-lookup"><span data-stu-id="faccd-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="faccd-108">A munkafolyamat futtatásakor a rendszer nem küldi el az e-mailt, és a következő viselkedést veszi észre:</span><span class="sxs-lookup"><span data-stu-id="faccd-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="faccd-109">A SharePoint 2013 platformtípust használó munkafolyamatok esetén keresse meg a **Munkafolyamat állapota** lapot.</span><span class="sxs-lookup"><span data-stu-id="faccd-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="faccd-110">A Munkafolyamat állapota lapon a **Belső állapot** beállítása **Elindítva**, és az információs buborék ban látható **A nem küldhető el a címzettnek**.</span><span class="sxs-lookup"><span data-stu-id="faccd-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="faccd-111">A probléma kerülő megoldásához konfigurálja úgy a munkafolyamatot, hogy az [Exchange Online feladói korlátainak](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)túllépése nélkül küldjön e-maileket.</span><span class="sxs-lookup"><span data-stu-id="faccd-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="faccd-112">Például szüneteltetheti a munkafolyamatot, elküldheti az e-mailt egy Microsoft 365-csoportnak, egy terjesztési csoportnak vagy egy levelezést engedélyező biztonsági csoportnak, vagy egyszerre kevesebb mint 200 címzettnek.</span><span class="sxs-lookup"><span data-stu-id="faccd-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="faccd-113">További információt a következő [cikkben](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)talál.</span><span class="sxs-lookup"><span data-stu-id="faccd-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="faccd-114">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="faccd-114">Related topics</span></span>
- [<span data-ttu-id="faccd-115">Folyamat létrehozása</span><span class="sxs-lookup"><span data-stu-id="faccd-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="faccd-116">SharePoint és Folyamat</span><span class="sxs-lookup"><span data-stu-id="faccd-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 