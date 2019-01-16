---
title: Hozzáférés megtagadva a munkafolyamat megtekintésekor
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293305"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="87b20-102">Hozzáférés megtagadva a munkafolyamat megtekintésekor</span><span class="sxs-lookup"><span data-stu-id="87b20-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="87b20-103">Kísérli meg egy e-mailt küldhet egy SharePoint-csoporthoz SharePoint 2013 munkafolyamatok "Hozzáférés megtagadva" hibaüzenettel sikertelen lehet, ha a SharePoint-csoport tagjainak van mindenki számára.</span><span class="sxs-lookup"><span data-stu-id="87b20-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="87b20-104">**A probléma megoldásához hajtsa végre ezeket a lépéseket:**</span><span class="sxs-lookup"><span data-stu-id="87b20-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="87b20-105">Lehetővé teszi mindenki megtekintheti a SharePoint-csoport tagjai.</span><span class="sxs-lookup"><span data-stu-id="87b20-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="87b20-106">A SharePoint-csoport eltávolítása a címzett vagy másolatot kap sor az e-mail.</span><span class="sxs-lookup"><span data-stu-id="87b20-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="87b20-107">Explicit módon vegye fel a címzett vagy másolatot kap sor, ha a SharePoint-csoport tagság láthatósága nem módosítható.</span><span class="sxs-lookup"><span data-stu-id="87b20-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="87b20-108">Megtekintése további részletekért olvassa el [/_vti_bin/client.svc/sp.utilities.utility.SendEmail a nem hitelesített HTTP ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="87b20-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

