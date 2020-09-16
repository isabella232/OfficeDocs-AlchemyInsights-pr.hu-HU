---
title: A napi e-mail-korlát túllépve. A munkafolyamat fel van függesztve.
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
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731565"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="87f53-103">A napi e-mail-korlát túllépve.</span><span class="sxs-lookup"><span data-stu-id="87f53-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="87f53-104">A munkafolyamat fel van függesztve.</span><span class="sxs-lookup"><span data-stu-id="87f53-104">Workflow is suspended.</span></span>

<span data-ttu-id="87f53-105">A hiba az alábbi esetekben fogadható el:</span><span class="sxs-lookup"><span data-stu-id="87f53-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="87f53-106">Munkafolyamata van a SharePoint Online-ban, amely a SharePoint 2010 vagy a SharePoint 2013 munkafolyamat platform típusát használja.</span><span class="sxs-lookup"><span data-stu-id="87f53-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="87f53-107">A munkafolyamat úgy van konfigurálva, hogy az egyéni e-mail-üzeneteket több mint 200-felhasználónál, naponta több mint 10 000 címzett, vagy percenként több mint 30 üzenetet küldjön.</span><span class="sxs-lookup"><span data-stu-id="87f53-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="87f53-108">A munkafolyamat futtatásakor az e-maileket nem küldi el a program, és a következő viselkedést tapasztalja:</span><span class="sxs-lookup"><span data-stu-id="87f53-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="87f53-109">Ha a munkafolyamathoz a SharePoint 2013 platformját használja, tallózással keresse meg a **munkafolyamat állapota** lapot.</span><span class="sxs-lookup"><span data-stu-id="87f53-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="87f53-110">A Munkafolyamat állapota lapon a **belső állapot** az **Indítás**értékre van állítva, az információs buborék pedig **nem tud elküldeni a címzetteknek**.</span><span class="sxs-lookup"><span data-stu-id="87f53-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="87f53-111">A probléma megoldásához állítsa be úgy a munkafolyamatot, hogy e-mail-üzeneteket küldjön az [Exchange Online-beli feladó korlátozásainak](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)túllépése nélkül.</span><span class="sxs-lookup"><span data-stu-id="87f53-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="87f53-112">Használhatja például a munkafolyamatban a szünetet, elküldheti az e-mailt egy Microsoft 365-csoportba, egy terjesztési csoportba vagy egy levelezési biztonsági csoportba, vagy elküldheti az üzenetet legalább 200 címzettnek.</span><span class="sxs-lookup"><span data-stu-id="87f53-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="87f53-113">További információt a következő [cikkben](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)talál.</span><span class="sxs-lookup"><span data-stu-id="87f53-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="87f53-114">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="87f53-114">Related topics</span></span>
- [<span data-ttu-id="87f53-115">Folyamatábra létrehozása</span><span class="sxs-lookup"><span data-stu-id="87f53-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="87f53-116">SharePoint és flow</span><span class="sxs-lookup"><span data-stu-id="87f53-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 