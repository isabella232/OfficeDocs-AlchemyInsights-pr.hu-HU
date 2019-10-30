---
title: Bevezetés a SharePoint Online használatbaveléshez
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766893"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="1df2a-102">Munkafolyamatok a SharePoint rendszerben</span><span class="sxs-lookup"><span data-stu-id="1df2a-102">Workflows in SharePoint</span></span>

<span data-ttu-id="1df2a-103">Ha a SharePoint-munkafolyamatok nem küldenek e-maileket, elképzelhető, hogy szervezete az Exchange Online feladójának korlátait észlelte.</span><span class="sxs-lookup"><span data-stu-id="1df2a-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="1df2a-104">A "munkafolyamat felfüggesztve" hibaüzenet akkor jelenhet meg, ha a következő elemek valamelyike fennáll:</span><span class="sxs-lookup"><span data-stu-id="1df2a-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="1df2a-105">Olyan munkafolyamatot használ a SharePoint Online szolgáltatásban, amely a SharePoint 2010 vagy SharePoint 2013 munkafolyamat-platformtípust használja.</span><span class="sxs-lookup"><span data-stu-id="1df2a-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="1df2a-106">A munkafolyamat úgy van beállítva, hogy egy egyéni e-mail üzenetet több mint 200 felhasználók részére küld egy időben, több mint 10 000 címzettek naponta, vagy több mint 30 üzenet percenként.</span><span class="sxs-lookup"><span data-stu-id="1df2a-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="1df2a-107">A munkafolyamat futtatásakor az e-mail üzenet nem kerül elküldésre, és a hibaüzenet jelenik meg, a belső állapot beállítás felfüggesztve, vagy a címzettnek nem lehet elküldeni a címzettet.</span><span class="sxs-lookup"><span data-stu-id="1df2a-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="1df2a-108">További információért lásd a következő [cikket](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="1df2a-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

