---
title: A külső felhasználókkal való megosztás nem működik
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502233"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>A SharePoint-tartalom külső felhasználókkal való megosztását szolgáló problémák megoldása

Győződjön meg arról, hogy a szervezeten belül be van kapcsolva a külső megosztás:
  
1. Keresse fel a [Microsoft &amp; 365 felügyeleti központ szolgáltatások bővítmények lapját](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), és kattintson a **helyek**gombra.
    
2. Ellenőrizze, hogy a beállítás be van-e kapcsolva. Ha a "csak meglévő külső felhasználók" beállítás van kijelölve, ellenőrizze, hogy a külső felhasználó szerepel-e a Microsoft 365 felügyeleti központban.
    
Ellenőrizze, hogy be van-e kapcsolva a webhely külső megosztása. Részére egy klasszikus telek gyűjtemény:
  
1. Az új SharePoint admin központban kattintson a bal oldali ablaktáblán a **helyek**elemre.
    
2. Jelölje ki a webhelyet vagy webhelyeket, majd a szalagon kattintson a **megosztás**elemre.
    
Office 365-csoporthoz vagy kommunikációs webhelyhez tartozó csoportwebhely esetén:
  
- Az új webhelytípusokhoz ugyanaz a megosztási beállítás van, mint a szervezeti szinten, kivéve, ha az egész szervezetre vonatkozó beállítás lehetővé teszi fájlok megosztását olyan hivatkozások segítségével, amelyekhez nem szükséges bejelentkezés. Ebben az esetben a webhelyek lehetővé teszik a megosztást új és meglévő külső felhasználókkal, akik bejelentkeznek. Az adott helyek beállításának megváltoztatásához használja az új SharePoint admin központot vagy a PowerShell parancshéjat. [További információ](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Az egyes webhelyek külső megosztási beállításai korlátozóbbak lehetnek, mint a szervezet egészére kiterjedő beállítások, de a szervezet egészére érvényes beállítás esetében nem megengedőbb. 
  

