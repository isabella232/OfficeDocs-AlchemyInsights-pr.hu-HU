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
# <a name="access-denied-when-viewing-a-workflow"></a>A munkafolyamatok megtekintésekor a hozzáférés megtagadva

SharePoint 2013 a SharePoint-csoportnak e-mailt küldeni próbálő munkafolyamatok "hozzáférés megtagadva" hibaüzenetet küldhetnek, ha a SharePoint-csoport tagsága nem mindenki értékre van állítva.
  
 **A probléma megoldásához hajtsa a következő lépéseket:**
  
 1. Engedélyezze, hogy mindenki lássa a SharePoint-csoport tagjait.
  
 2. Távolítsa el a SharePoint-csoportot az e-mail Címzett vagy másolatot kap sorába.
  
 3. Ha a tagság láthatóságát a SharePoint-csoport esetében nem lehet módosítani, explicit módon adja hozzá a felhasználókat a címzett vagy a másolatot kap sorhoz.
  
További részletekért lásd a [http jogosulatlan a/_vti_bin/Client.SVC/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  