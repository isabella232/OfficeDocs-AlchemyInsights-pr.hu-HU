---
title: Hozzáférés korlátozása a SharePointban vagy a OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720684"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hozzáférés korlátozása a SharePointban vagy a OneDrive

A SharePointban és a OneDrive a hozzáférést csak olyan csoportoknak vagy magánszemélyeknek engedélyezi, akiknek hozzáférése van. Alapértelmezés szerint az engedélyek a SharePointban a hierarchia magasabb szintjéről öröklődnek. Így a fájlok öröklik az engedélyeket a mappából, amely örökli az engedélyeit a tárból, ami örökli az engedélyeit a webhelyről.
  
Megoszthat magasabb szintre (például egy teljes webhely megosztásával), majd megszakíthatja az öröklést, ha nem szeretné megosztani a webhely összes elemét. Ezt azonban nem javasoljuk, mert az engedélyeket a jövőben összetettebbvé és zavarosnak tartja. Az alábbi műveleteket végezheti el:
  
- Ha például egy mappa teljes tartalmát szeretné megosztani, kivéve az egyik fájlt, helyezze át a fájlt egy olyan új helyre, amely nincs megosztva.
    
- Ha egy mappában két almappája van, és egy almappát szeretne megosztani az A és A B csoporttal, és csak a második almappához szeretne hozzáférést engedélyezni, ossza meg a szülőmappa az A és b csoporttal, és vegye fel a B csoportot az első almappába.
    
[Fájl vagy mappa megosztásának megszüntetése ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

