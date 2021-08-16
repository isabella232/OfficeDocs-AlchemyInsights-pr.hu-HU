---
title: Hozzáférés korlátozása a SharePoint-ban OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075042"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hozzáférés korlátozása a SharePoint-ban OneDrive

A SharePoint és a OneDrive úgy korlátozza a hozzáférést az elemekhez, például fájlokhoz, mappákhoz és listákhoz, hogy csak azoknak a csoportoknak vagy személyeknek biztosít hozzáférést, akikhez hozzáférést szeretne. Alapértelmezés szerint a SharePoint a hierarchia magasabbról örökli az engedélyeket. A fájlok tehát öröklik az engedélyeket a mappától, amely a tártól örökli az engedélyeket, amely a webhelytől örökli az engedélyeket.
  
A megosztás magasabb szinten történik (például egy teljes webhely megosztásával), majd megszakíthatja az öröklést, ha nem szeretné a webhely minden elemét megosztani. Ezt azonban nem javasoljuk, mert ez bonyolultabb és zavarosabb lesz a jövőben. Ehelyett a következőt tehet:
  
- Ha például egy mappa teljes tartalmát szeretné megosztani, kivéve egy fájlt, helyezze át a fájlt egy olyan új helyre, amely nincs megosztva.
    
- Ha egy mappában két almappa található, és meg szeretné osztani az egyik almappát az A és a B csoporttal, és csak az A csoportnak szeretné engedélyezni a hozzáférést a második almappába, ossza meg a szülőmappát az A csoporttal, és adja hozzá a B csoportot az első almappába.
    
[Fájl vagy mappa megosztásának törlése ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

