---
title: Megnyitás Explorer nem működik
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764910"
---
# <a name="open-with-explorer-isnt-working"></a>Megnyitás Explorer nem működik

Ha nem működik a **Megnyitás Intézővel** vagy **az Intéző nézetben** ellenőrizze, hogy a WebClient szolgáltatás **futtatásához** van beállítva, az alábbi lépéseket követve. Például ha a szolgáltatás nem fut a SharePoint vagy a OneDrive könyvtár megnyitása hosszú ideig is eltarthat. 
  
1. A Windows keresési mezőjében típus futtatni, jelölje be a Futtatás asztali alkalmazás, típus services.msc és majd **Enter**.
    
2. Görgessen le a webes ügyfélszolgáltatást, és ellenőrizze az **állapot** oszlopban. A WebClient szolgáltatás állapota nem **fut**, kattintson duplán a szolgáltatásra, kattintson a **Start menüre**és kattintson az **OK gombra**. A szolgáltatás engedélyezése, ha szükséges, az **Indítás típusa** mezőben a **kézi** vagy **automatikus** kiválasztásával. 
    
> [!NOTE]
> Explorer fájl megnyitásával kapcsolatos problémák elhárítása, lásd: [Nyissa meg az Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Fedezze fel a Szinkronizáló jobb alternatíva: [az új OneDrive szinkronizálás ügyfél fájlok szinkronizálása SharePoint](https://go.microsoft.com/fwlink/?linkid=871666). 
  

