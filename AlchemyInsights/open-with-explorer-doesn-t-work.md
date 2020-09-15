---
title: A Megnyitás Intézővel parancs nem működik
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694458"
---
# <a name="open-with-explorer-isnt-working"></a>A Megnyitás Intézővel nem végezhető műveletek

Ha a **Megnyitás Intézővel** vagy a **megtekintés a Fájlkezelőben** parancs nem működik, győződjön meg arról **, hogy a** WebClient szolgáltatás az alábbi lépésekkel van beállítva. Hosszú időbe telik például a SharePoint-vagy OneDrive-tár megnyitása, ha a szolgáltatás nem fut. 
  
1. A Windows Search mezőbe írja be a Futtatás parancsot, és válassza az asztali Futtatás alkalmazást, írja be a Services. msc parancsot, és válassza az **ENTER billentyűt**.
    
2. Görgessen le a WebClient szolgáltatáshoz, és ellenőrizze az **állapot** oszlopot. Ha a WebClient szolgáltatás állapota nem **fut**, kattintson duplán a szolgáltatásra, kattintson a **Start**gombra, majd **az OK**gombra. Engedélyezze a szolgáltatást, ha szükséges, az **indítási típus** mezőben válassza a **kézi** vagy az **automatikus** lehetőséget. 
    
> [!NOTE]
> A Fájlkezelőben való megnyitással kapcsolatos hibák elhárításáról a [Megnyitás az Intézőben](https://go.microsoft.com/fwlink/?linkid=871665)című témakörben olvashat. A szinkronizálás megismerése jobb alternatíva: [SharePoint-fájlok szinkronizálása az új OneDrive szinkronizálási ügyfélprogrammal](https://go.microsoft.com/fwlink/?linkid=871666). 
  

