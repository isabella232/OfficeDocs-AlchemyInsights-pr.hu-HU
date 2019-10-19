---
title: Hozzáférés korlátozása a SharePoint vagy az OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551453"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hozzáférés korlátozása a SharePoint vagy az OneDrive

A SharePoint és az OneDrive alkalmazásban a fájlokhoz, mappákhoz és listákhoz hasonló elemekhez való hozzáférést úgy korlátozhatja, hogy csak az elérni kívánt csoportoknak vagy személyeknek biztosít hozzáférést. Alapértelmezés szerint a SharePoint rendszerben az engedélyek a hierarchiában feljebb lévő jogosultságoktól öröklődnek. Tehát egy fájl örökli a jogosultságokat a mappából, amely örökli a jogosultságokat a könyvtár, amely örökli a jogosultságokat a hely.
  
A megosztást magasabb szinten (például egy egész webhely megosztásával) megoszthatja, majd az öröklődés megszakadhat, ha nem szeretné megosztani a webhely összes elemét. Azonban ezt nem javasoljuk, mert a jogosultságokat a jövőben bonyolultabbá és bonyolultabbá teszi. Itt van, mit lehetne csinálni helyette:
  
- Ha például egy mappa teljes tartalmát meg szeretné osztani egy fájlon kívül, helyezze át a fájlt egy olyan új helyre, amely nincs megosztva.
    
- Ha egy mappában két almappája van, és egy almappát szeretne megosztani az A és A B csoporttal, és csak az A csoport férhet hozzá a második almappához, ossza meg a szülőmappát az A csoporttal, és az első almappához vegye fel a B csoportot.
    
[Fájl vagy mappa megosztásának leállítása](https://go.microsoft.com/fwlink/?linkid=2008861)
  

