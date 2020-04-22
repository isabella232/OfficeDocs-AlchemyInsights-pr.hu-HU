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
# <a name="access-denied-when-viewing-a-workflow"></a>Hozzáférés megtagadva munkafolyamat megtekintésekor

Azok a SharePoint 2013-munkafolyamatok, amelyek e-mailt próbálnak küldeni egy SharePoint-csoportnak, "Hozzáférés megtagadva" hibaüzenettel meghiúsulhatnak, ha a SharePoint-csoport tagsága nincs Mindenki.
  
 **A probléma megoldásához tegye a következőket:**
  
 1. A SharePoint-csoport tagjainak megtekintésének engedélyezése mindenki számára.
  
 2. Távolítsa el a SharePoint-csoportot az e-mail Címzett vagy MÁSOLATOT sorából.
  
 3. Explicit módon adja hozzá a felhasználókat a Címzett vagy a Másolatot kap sorhoz, ha a SharePoint-csoport tagsági láthatósága nem módosítható.
  
További részletek megtekintéséhez kérjük, olvassa el a [HTTP Jogosulatlan a /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  