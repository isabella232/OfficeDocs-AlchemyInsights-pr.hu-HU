---
title: Access denied when viewing a Workflow
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955203"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access denied when viewing a Workflow

SharePoint 2013-as munkafolyamatok, amelyek e-mailt próbálnak küldeni egy SharePoint-csoportnak, sikertelen lehet "Hozzáférés megtagadva" hibaüzenettel, ha a SharePoint-csoport tagsága nincs Mindenki beállításra állítva.
  
 **A probléma megoldásához kövesse az alábbi lépéseket:**
  
 1. Mindenki láthatja a csoport SharePoint tagokat.
  
 2. Távolítsa el SharePoint címzettcsoportot az e-mail Címzett vagy Másolatot kap sorában.
  
 3. Vegye fel kifejezetten a felhasználókat a Címzett vagy a Másolatot kap sorba, ha a tagság láthatósága nem módosítható SharePoint csoportban.
  
További részletekért olvassa el a [HTTP: /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)) címet.
  