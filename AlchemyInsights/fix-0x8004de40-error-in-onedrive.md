---
title: Erősít 0x8004de40 hiba-ban OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052039"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Erősít 0x8004de40 hiba-ban OneDrive

Ha 0x8004de40 jelű hibát kap az OneDrive esetében:

- Újraindít a érintett számítógép rövid idő összekapcsolt-hoz-a Acitve címtár birtok.
- Ha egy újraindítás nem oldja meg a problémát, akkor elválaszt, és csatlakoztassa a készüléket Azure ad. 

**Megjegyzés**: a lépések végrehajtása során a vállalati hálózaton kell lennie. Ne hajtsa végre ezeket a lépéseket, ha nem tud csatlakozni a vállalati infrastruktúrához (például utazás közben). 

- Nyit egyemelkedett követel gyors. 
- Az emelt szintű parancssor megnyitásához kattintson a **Start**gombra, kattintson a jobb gombbal **a parancssor elemre, majd**kattintson a **Futtatás rendszergazdaként**parancsra.
- Írja be a *dsregcmd/Leave* parancsot, majd nyomja le az **ENTER billentyűt**.
- Amikor elkészült, írja be a *dsregcmd/JOIN* parancsot, és nyomja meg az **ENTER**billentyűt.
- Ha elkészült, zárja be a parancssort.
- Újraindít a számítógép, és fatörzs-ba OneDrive.