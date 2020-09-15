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
# <a name="access-denied-when-viewing-a-workflow"></a>Hozzáférés megtagadva egy munkafolyamat megtekintésekor

A SharePoint-csoportokba érkező e-mailek küldését megkísérlő SharePoint-2013-munkafolyamatok "hozzáférés megtagadva" hibaüzenettel jelenhetnek meg, ha a SharePoint-csoport tagsága nincs mindenki számára beállítva.
  
 **A probléma megoldásához hajtsa végre az alábbi lépéseket:**
  
 1. Engedélyezze mindenki számára a SharePoint-csoport tagjainak a megjelenítését.
  
 2. Távolítsa el a SharePoint-csoportot az e-mail Címzett vagy másolatot kap sorából.
  
 3. Ha a tagság láthatósága nem módosítható a SharePoint-csoportban, explicit módon adja hozzá a felhasználókat a címzett vagy a másolatot kap sorban.
  
Ha további részleteket szeretne megtudni, olvassa el a [http – jogosulatlan _vti_bin/Client.SVC/SP.Utilities.Utility.sendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  