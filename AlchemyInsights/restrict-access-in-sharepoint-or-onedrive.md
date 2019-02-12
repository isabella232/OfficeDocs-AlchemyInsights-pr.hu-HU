---
title: Korlátozza a hozzáférést a SharePoint- vagy OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29905150"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Korlátozza a hozzáférést a SharePoint- vagy OneDrive

A SharePoint és a OneDrive tiltjuk meg elemekhez, például fájlok, mappák és listákat csak a csoportok vagy egyének szeretne hozzáférést nyújtó. Alapértelmezés szerint a SharePoint engedélyek hierarchiájában magasabb felfelé öröklődnek. Így a fájl az engedélyeit örökli a mappából, amelynek az engedélyeit örökli a műsortárból, amelynek az engedélyeit örökli a webhelyről.
  
Megoszthatja a magasabb szintű (például egy teljes webhelyet megosztásával) és majd öröklődés megszakítása, ha nem szeretnénk megosztani a webhely elemeinek. Azonban nem ajánlott ez mert így fenntartása az engedélyeket több összetettnek és zavarosnak a jövőben. Íme, mit sikerült helyette tenni:
  
- Ha például szeretne megosztani egy mappát, kivéve egy fájl tartalmát, helyezze át ezt a fájlt olyan helyre, amely nem osztott.
    
- Ha egy mappában vannak almappák két, és szeretné megosztani egy almappát a és B csoportba és hozzáférést csak A csoport második almappájába, a mappa megosztása A csoport és a B csoport hozzáadása az első almappa.
    
[Fájl vagy mappa megosztásának megszüntetése](https://go.microsoft.com/fwlink/?linkid=2008861)
  

