---
title: Korlátozza a hozzáférést a SharePoint- vagy OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293855"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Korlátozza a hozzáférést a SharePoint- vagy OneDrive

A SharePoint és a OneDrive tiltjuk meg elemekhez, például fájlok, mappák és listákat csak a csoportok vagy egyének szeretne hozzáférést nyújtó. Alapértelmezés szerint a SharePoint engedélyek hierarchiájában magasabb felfelé öröklődnek. Így a fájl az engedélyeit örökli a mappából, amelynek az engedélyeit örökli a műsortárból, amelynek az engedélyeit örökli a webhelyről.
  
Megoszthatja a magasabb szintű (például egy teljes webhelyet megosztásával) és majd öröklődés megszakítása, ha nem szeretnénk megosztani a webhely elemeinek. Azonban nem ajánlott ez mert így fenntartása az engedélyeket több összetettnek és zavarosnak a jövőben. Íme, mit sikerült helyette tenni:
  
- Ha például szeretne megosztani egy mappát, kivéve egy fájl tartalmát, helyezze át ezt a fájlt olyan helyre, amely nem osztott.
    
- Ha egy mappában vannak almappák két, és szeretné megosztani egy almappát a és B csoportba és hozzáférést csak A csoport második almappájába, a mappa megosztása A csoport és a B csoport hozzáadása az első almappa.
    
[Fájl vagy mappa megosztásának megszüntetése](https://go.microsoft.com/fwlink/?linkid=2008861)
  

