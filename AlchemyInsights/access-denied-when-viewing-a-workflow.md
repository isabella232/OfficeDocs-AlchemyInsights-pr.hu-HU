---
title: Hozzáférés megtagadva a munkafolyamat megtekintésekor
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883593"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="24cbd-102">Hozzáférés megtagadva a munkafolyamat megtekintésekor</span><span class="sxs-lookup"><span data-stu-id="24cbd-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="24cbd-103">Kísérli meg egy e-mailt küldhet egy SharePoint-csoporthoz SharePoint 2013 munkafolyamatok "Hozzáférés megtagadva" hibaüzenettel sikertelen lehet, ha a SharePoint-csoport tagjainak van mindenki számára.</span><span class="sxs-lookup"><span data-stu-id="24cbd-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="24cbd-104">**A probléma megoldásához hajtsa végre ezeket a lépéseket:**</span><span class="sxs-lookup"><span data-stu-id="24cbd-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="24cbd-105">Lehetővé teszi mindenki megtekintheti a SharePoint-csoport tagjai.</span><span class="sxs-lookup"><span data-stu-id="24cbd-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="24cbd-106">A SharePoint-csoport eltávolítása a címzett vagy másolatot kap sor az e-mail.</span><span class="sxs-lookup"><span data-stu-id="24cbd-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="24cbd-107">Explicit módon vegye fel a címzett vagy másolatot kap sor, ha a SharePoint-csoport tagság láthatósága nem módosítható.</span><span class="sxs-lookup"><span data-stu-id="24cbd-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="24cbd-108">Megtekintése további részletekért olvassa el [/_vti_bin/client.svc/sp.utilities.utility.SendEmail a nem hitelesített HTTP](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="24cbd-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  