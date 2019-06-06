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
ms.openlocfilehash: a44b2c7b26895e09c24df772f1ada9a2e3483747
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735985"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="5872b-102">A SharePoint munkafolyamatok</span><span class="sxs-lookup"><span data-stu-id="5872b-102">Workflows in SharePoint</span></span>

<span data-ttu-id="5872b-103">Ha a SharePoint-munkafolyamatok nem küldött e-mailek, valószínűleg a szervezet észlelt küldő Exchange Online keretein.</span><span class="sxs-lookup"><span data-stu-id="5872b-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="5872b-104">"A munkafolyamat fel van függesztve" hibaüzenet is fordul elő, ha a következő elemek egyikét:</span><span class="sxs-lookup"><span data-stu-id="5872b-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="5872b-105">A munkafolyamat a SharePoint Online használja a SharePoint 2010 vagy a SharePoint 2013 munkafolyamat platformtípusa van.</span><span class="sxs-lookup"><span data-stu-id="5872b-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="5872b-106">A munkafolyamat egyéni e-mail üzenetet küldhet a felhasználók több mint 200 egyszerre, naponta 10 000-nél több címzettnek vagy egy perc alatt több mint 30 üzenetnél van beállítva.</span><span class="sxs-lookup"><span data-stu-id="5872b-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="5872b-107">Amikor futtatja a munkafolyamatot, az e-mailt nem küldi el, és azt tapasztalja, hogy a hibaüzenet, belső beállítás egy címzettnek küldendő Suspended, vagy nem jelenik meg.</span><span class="sxs-lookup"><span data-stu-id="5872b-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="5872b-108">További információért olvassa el a következő [cikk](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="5872b-108">For more information, please refer to the following [article](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

