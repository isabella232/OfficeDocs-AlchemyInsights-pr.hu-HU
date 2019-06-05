---
title: A SharePoint Online Ismerkedés
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 9a8d72a01ed35794fcab370b48bbb189663d3396
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34718749"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="57736-102">A SharePoint munkafolyamatok</span><span class="sxs-lookup"><span data-stu-id="57736-102">Workflows in SharePoint</span></span>

<p><span data-ttu-id="57736-103">Ha a SharePoint-munkafolyamatok nem küldött e-mailek, valószínűleg a szervezet észlelt küldő Exchange Online keretein.&nbsp;</span><span class="sxs-lookup"><span data-stu-id="57736-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.&nbsp;</span></span></p> <p><span data-ttu-id="57736-104">"A munkafolyamat fel van függesztve" hibaüzenet is fordul elő, ha a következő elemek egyikét:</span><span class="sxs-lookup"><span data-stu-id="57736-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span></p> <ul> <li><span data-ttu-id="57736-105">A munkafolyamat a SharePoint Online használja a SharePoint 2010 vagy a SharePoint 2013 munkafolyamat platformtípusa van.</span><span class="sxs-lookup"><span data-stu-id="57736-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span></li> <li><span data-ttu-id="57736-106">A munkafolyamat egyéni e-mail üzenetet küldhet a felhasználók több mint 200 egyszerre, naponta 10 000-nél több címzettnek vagy egy perc alatt több mint 30 üzenetnél van beállítva.</span><span class="sxs-lookup"><span data-stu-id="57736-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span></li> <li><span data-ttu-id="57736-107">Amikor futtatja a munkafolyamatot, az e-mailt nem küldi el, és azt tapasztalja, hogy a hibaüzenet jelenik meg, és <strong>belső állapot Suspended meg</strong> <strong>nem sikerült elküldeni a címzetthez</strong> jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="57736-107">When you run the workflow, the email message isn't sent, and you notice the error message, <strong>Internal Status is set to Suspended</strong> or <strong>Unable to send to a recipient</strong> is displayed.</span></span></li> </ul> <p><span data-ttu-id="57736-108">További információért olvassa el a következő <a href="https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US">cikk</a>.</span><span class="sxs-lookup"><span data-stu-id="57736-108">For more information, please refer to the following <a href="https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US">article</a>.</span></span></p>

