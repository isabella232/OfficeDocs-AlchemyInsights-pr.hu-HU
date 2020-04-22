---
title: Hozzáférés korlátozása a SharePointban vagy a OneDrive-on
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715886"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hozzáférés korlátozása a SharePointban vagy a OneDrive-on

A SharePointban és a OneDrive-ban korlátozhatja a hozzáférést az olyan elemekhez, mint a fájlok, mappák és listák, mivel csak olyan csoportoknak vagy személyeknek biztosít hozzáférést, amelyekhez hozzá szeretne férni. Alapértelmezés szerint a SharePoint engedélyei a hierarchia magasabb szintű részétől öröklődnek. Így egy fájl örökli az engedélyeit a mappából, amely az engedélyeket a tárból örökli, amely az engedélyeket a webhelytől örökli.
  
Magasabb szinten is megoszthatja (például egy teljes webhely megosztásával), majd megszakíthatja az öröklődést, ha nem szeretné megosztani a webhely összes elemét. Ezt azonban nem javasoljuk, mert a jövőben bonyolultabbá és zavarosabbá teszi az engedélyek karbantartását. Ehelyett a következőket teheti:
  
- Ha például egy mappa teljes tartalmát meg szeretné osztani, kivéve egy fájlt, helyezze át a fájlt egy új helyre, amely nincs megosztva.
    
- Ha egy mappában két almappa van, és egy almappát meg szeretne osztani az A és B csoporttal, és csak az A csoport számára engedélyezi a hozzáférést a második almappához, ossza meg a szülőmappát az A csoporttal, és adja hozzá a B csoportot az első almappához.
    
[Fájl vagy mappa megosztásának leállítása](https://go.microsoft.com/fwlink/?linkid=2008861)
  

