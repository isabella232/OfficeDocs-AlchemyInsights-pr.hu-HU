---
title: A munkafolyamatok megtekintésekor a hozzáférés megtagadva
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747750"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="d5236-102">A munkafolyamatok megtekintésekor a hozzáférés megtagadva</span><span class="sxs-lookup"><span data-stu-id="d5236-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="d5236-103">SharePoint 2013 a SharePoint-csoportnak e-mailt küldeni próbálő munkafolyamatok "hozzáférés megtagadva" hibaüzenetet küldhetnek, ha a SharePoint-csoport tagsága nem mindenki értékre van állítva.</span><span class="sxs-lookup"><span data-stu-id="d5236-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="d5236-104">**A probléma megoldásához hajtsa a következő lépéseket:**</span><span class="sxs-lookup"><span data-stu-id="d5236-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="d5236-105">Engedélyezze, hogy mindenki lássa a SharePoint-csoport tagjait.</span><span class="sxs-lookup"><span data-stu-id="d5236-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="d5236-106">Távolítsa el a SharePoint-csoportot az e-mail Címzett vagy másolatot kap sorába.</span><span class="sxs-lookup"><span data-stu-id="d5236-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="d5236-107">Ha a tagság láthatóságát a SharePoint-csoport esetében nem lehet módosítani, explicit módon adja hozzá a felhasználókat a címzett vagy a másolatot kap sorhoz.</span><span class="sxs-lookup"><span data-stu-id="d5236-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="d5236-108">További részletekért lásd a [http jogosulatlan a/_vti_bin/Client.SVC/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="d5236-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  