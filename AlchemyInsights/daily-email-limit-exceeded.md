---
title: Napi e-mail határ túllépése. A munkafolyamat fel van függesztve.
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
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514457"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="b64d5-103">Napi e-mail túllépi a megengedettet.</span><span class="sxs-lookup"><span data-stu-id="b64d5-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="b64d5-104">A munkafolyamat fel van függesztve.</span><span class="sxs-lookup"><span data-stu-id="b64d5-104">Workflow is suspended.</span></span>

<span data-ttu-id="b64d5-105">Ez a hiba megérkezhetnek az alábbi esetekben:</span><span class="sxs-lookup"><span data-stu-id="b64d5-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="b64d5-106">A munkafolyamat a SharePoint Online használja a SharePoint 2010 vagy a SharePoint 2013 munkafolyamat platformtípusa van.</span><span class="sxs-lookup"><span data-stu-id="b64d5-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="b64d5-107">A munkafolyamat egyéni e-mail üzenetet küldhet a felhasználók több mint 200 egyszerre, naponta 10 000-nél több címzettnek vagy egy perc alatt több mint 30 üzenetnél van beállítva.</span><span class="sxs-lookup"><span data-stu-id="b64d5-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="b64d5-108">Amikor futtatja a munkafolyamatot, az e-mailt nem küldi el, és azt tapasztalja, hogy a következőképp működik:</span><span class="sxs-lookup"><span data-stu-id="b64d5-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="b64d5-109">A munkafolyamat segítségével a SharePoint 2013 platform típusa akkor keresse meg a **Munkafolyamat állapota** lapon.</span><span class="sxs-lookup"><span data-stu-id="b64d5-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="b64d5-110">A munkafolyamat állapota oldalon **Belső állapota** **Elindítva**értékre van állítva, és az információs buborékban **nem sikerült elküldeni a címzetthez**.</span><span class="sxs-lookup"><span data-stu-id="b64d5-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="b64d5-111">A probléma kerülő megoldásához állítsa be a munkafolyamat e-mailek küldése a [küldő Exchange Online korlátok](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)túllépése nélkül.</span><span class="sxs-lookup"><span data-stu-id="b64d5-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="b64d5-112">Például használja a munkafolyamat szünetet, az e-mailt küld egy Office 365, a terjesztési csoport vagy engedélyezett levelezési biztonsági csoport, vagy küldje el az üzenetet a címzetteknek kevesebb, mint 200 egyszerre.</span><span class="sxs-lookup"><span data-stu-id="b64d5-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="b64d5-113">További információt a következő [cikkben](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)talál.</span><span class="sxs-lookup"><span data-stu-id="b64d5-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="b64d5-114">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="b64d5-114">Related topics</span></span>
- [<span data-ttu-id="b64d5-115">Folyamat létrehozása</span><span class="sxs-lookup"><span data-stu-id="b64d5-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="b64d5-116">A SharePoint és az áram</span><span class="sxs-lookup"><span data-stu-id="b64d5-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 