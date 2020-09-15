---
title: SharePoint Online – első lépések
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700709"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="4fe88-102">SharePoint-munkafolyamatok</span><span class="sxs-lookup"><span data-stu-id="4fe88-102">Workflows in SharePoint</span></span>

<span data-ttu-id="4fe88-103">Ha a SharePoint-munkafolyamatok nem küldenek e-maileket, előfordulhat, hogy szervezete találkozott az Exchange Online-beli meghívóhoz tartozó korlátozásokkal.</span><span class="sxs-lookup"><span data-stu-id="4fe88-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="4fe88-104">A munkafolyamatot felfüggesztő hibaüzenet akkor fordulhat elő, ha az alábbi elemek egyike van:</span><span class="sxs-lookup"><span data-stu-id="4fe88-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="4fe88-105">Munkafolyamata van a SharePoint Online-ban, amely a SharePoint 2010 vagy a SharePoint 2013 munkafolyamat platform típusát használja.</span><span class="sxs-lookup"><span data-stu-id="4fe88-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="4fe88-106">A munkafolyamat úgy van konfigurálva, hogy az egyéni e-mail-üzeneteket több mint 200-felhasználónál, naponta több mint 10 000 címzett, vagy percenként több mint 30 üzenetet küldjön.</span><span class="sxs-lookup"><span data-stu-id="4fe88-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="4fe88-107">Ha futtatja a munkafolyamatot, a rendszer nem küldi el az e-mailt, és a hibaüzenet jelenik meg, a belső állapot beállítás felfüggesztve vagy nem küldhető címzettnek.</span><span class="sxs-lookup"><span data-stu-id="4fe88-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="4fe88-108">További információért olvassa el a következő [cikket](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="4fe88-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

