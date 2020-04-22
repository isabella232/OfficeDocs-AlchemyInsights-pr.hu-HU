---
title: Hozzáférés megtagadva munkafolyamat megtekintésekor
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687332"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="dcf4c-102">Hozzáférés megtagadva munkafolyamat megtekintésekor</span><span class="sxs-lookup"><span data-stu-id="dcf4c-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="dcf4c-103">Azok a SharePoint 2013-munkafolyamatok, amelyek e-mailt próbálnak küldeni egy SharePoint-csoportnak, "Hozzáférés megtagadva" hibaüzenettel meghiúsulhatnak, ha a SharePoint-csoport tagsága nincs Mindenki.</span><span class="sxs-lookup"><span data-stu-id="dcf4c-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="dcf4c-104">**A probléma megoldásához tegye a következőket:**</span><span class="sxs-lookup"><span data-stu-id="dcf4c-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="dcf4c-105">A SharePoint-csoport tagjainak megtekintésének engedélyezése mindenki számára.</span><span class="sxs-lookup"><span data-stu-id="dcf4c-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="dcf4c-106">Távolítsa el a SharePoint-csoportot az e-mail Címzett vagy MÁSOLATOT sorából.</span><span class="sxs-lookup"><span data-stu-id="dcf4c-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="dcf4c-107">Explicit módon adja hozzá a felhasználókat a Címzett vagy a Másolatot kap sorhoz, ha a SharePoint-csoport tagsági láthatósága nem módosítható.</span><span class="sxs-lookup"><span data-stu-id="dcf4c-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="dcf4c-108">További részletek megtekintéséhez kérjük, olvassa el a [HTTP Jogosulatlan a /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="dcf4c-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  