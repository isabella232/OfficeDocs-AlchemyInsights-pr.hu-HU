---
title: Erősít 0x8004de40 hiba-ban OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755850"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Erősít 0x8004de40 hiba-ban OneDrive

Ha 0x8004de40 hibakódot kap az OneDrive-nál:

- Újraindít a érintett számítógép rövid idő összekapcsolt-hoz-a Acitve címtár birtok.
- Ha egy újraindítás nem oldja meg a problémát, akkor elválaszt, és csatlakoztassa a készüléket Azure ad. 

**Megjegyzés**: a lépések végrehajtása során a vállalati hálózaton kell lennie. Ne hajtsa végre ezeket a lépéseket, ha nem tud csatlakozni a vállalati infrastruktúrához (például utazás közben). 

- Nyit egyemelkedett követel gyors. 
- Az emelt szintű parancssor megnyitásához kattintson a **Start**gombra, kattintson a jobb gombbal **a parancssor elemre, majd**kattintson a **Futtatás rendszergazdaként**parancsra.
- Írja be a *dsregcmd/Leave* parancsot, majd nyomja le az **ENTER billentyűt**.
- Amikor elkészült, írja be a *dsregcmd/JOIN* parancsot, és nyomja meg az **ENTER**billentyűt.
- Ha elkészült, zárja be a parancssort.
- Újraindít a számítógép, és fatörzs-ba OneDrive.