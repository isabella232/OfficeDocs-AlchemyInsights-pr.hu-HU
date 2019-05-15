---
title: A modern webhelyre, ahol a legfelső szintű webhely
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057723"
---
# <a name="modern-site-as-root-site"></a>A modern webhelyre, ahol a legfelső szintű webhely

[Cél fontos](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) vevők most lehetővé teszi a modern kommunikációs webhely tapasztalatok a SharePoint bérlő által a klasszikus legfelső szintű helyen.

Ez a szolgáltatás egyszerű PowerShell parancsmag futtatásával aktiválható. A PowerShell command(s) sikeres végrehajtását a legfelső szintű webhely lesz a kommunikáció új webhely kezdőlapja. A cikk [Engedélyezése-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)PowerShell parancsmag és szolgáltatás követelményeiről részletesen érhetők el. 

Azt is kell fokozatosan működés közbeni, ez ki alapértelmezés szerint célzott kiadás korai május 2019, vevőkhöz és a roll ki lesz elérhető világszerte 2019 június végén. Továbbra is a [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) más új funkciókról a Modern hivatkozik. 

**Fontos**: ne törölje a klasszikus legfelső szintű webhely a modern kommunikációs webhelyet hozhat létre. Ez a Microsoft által nem támogatott. A legfelső szintű webhely törlése tesz minden SharePoint-webhely a szervezet nem érhető el minden felhasználó számára addig, amíg a webhely visszaállítása, vagy hozzon létre egy új helyet azonos URL-címen. 
 
 