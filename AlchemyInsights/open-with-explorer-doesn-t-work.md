---
title: Nem működik a Megnyitás az Intézővel
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713036"
---
# <a name="open-with-explorer-isnt-working"></a>Nem működik a Megnyitás az Intézővel

Ha **a Megnyitás explorerrel** vagy **a Fájlkezelőben való megtekintés** sel nem működik, ellenőrizze, hogy a WebClient szolgáltatás futása beállítással **fut-e** az alábbi lépések végrehajtásával. Ha például a szolgáltatás nem fut, hosszú időbe telhet egy SharePoint- vagy OneDrive-tár megnyitása. 
  
1. A Windows keresőmezőjében írja be a futtatás t, jelölje be az Asztali alkalmazás futtatása jelölőnégyzetet, írja be a services.msc parancsot, majd válassza **az Enter lehetőséget.**
    
2. Görgessen le a WebClient szolgáltatáshoz, és ellenőrizze az **Állapot** oszlopot. Ha a WebClient szolgáltatás állapota nem **fut,** kattintson duplán a szolgáltatásra, kattintson a **Start**gombra, majd az **OK**gombra. Szükség esetén engedélyezze a szolgáltatást az Indítás **típusa** mezőben a **Kézi** vagy az **Automatikus** lehetőséget. 
    
> [!NOTE]
> A Fájlkezelőben megnyitott problémák elhárításáról a [Megnyitás az Intézőben című témakörben](https://go.microsoft.com/fwlink/?linkid=871665)található. A szinkronizálás jobb alternatívaként való [felfedezése: SharePoint-fájlok szinkronizálása az új OneDrive szinkronizálási ügyfélalkalmazással](https://go.microsoft.com/fwlink/?linkid=871666). 
  

