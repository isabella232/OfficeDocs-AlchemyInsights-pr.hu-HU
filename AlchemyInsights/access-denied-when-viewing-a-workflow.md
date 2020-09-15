---
title: Hozzáférés megtagadva egy munkafolyamat megtekintésekor
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688804"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="9a254-102">Hozzáférés megtagadva egy munkafolyamat megtekintésekor</span><span class="sxs-lookup"><span data-stu-id="9a254-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="9a254-103">A SharePoint-csoportokba érkező e-mailek küldését megkísérlő SharePoint-2013-munkafolyamatok "hozzáférés megtagadva" hibaüzenettel jelenhetnek meg, ha a SharePoint-csoport tagsága nincs mindenki számára beállítva.</span><span class="sxs-lookup"><span data-stu-id="9a254-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="9a254-104">**A probléma megoldásához hajtsa végre az alábbi lépéseket:**</span><span class="sxs-lookup"><span data-stu-id="9a254-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="9a254-105">Engedélyezze mindenki számára a SharePoint-csoport tagjainak a megjelenítését.</span><span class="sxs-lookup"><span data-stu-id="9a254-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="9a254-106">Távolítsa el a SharePoint-csoportot az e-mail Címzett vagy másolatot kap sorából.</span><span class="sxs-lookup"><span data-stu-id="9a254-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="9a254-107">Ha a tagság láthatósága nem módosítható a SharePoint-csoportban, explicit módon adja hozzá a felhasználókat a címzett vagy a másolatot kap sorban.</span><span class="sxs-lookup"><span data-stu-id="9a254-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="9a254-108">Ha további részleteket szeretne megtudni, olvassa el a [http – jogosulatlan _vti_bin/Client.SVC/SP.Utilities.Utility.sendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="9a254-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  