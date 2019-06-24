---
title: A OneDrive 0x8004de40 hiba javítása
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133979"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>A OneDrive 0x8004de40 hiba javítása

Ha a OneDrive egy 0x8004de40 hibaüzenet jelenik meg:

- Indítsa újra a aktivizált Directory tartományhoz csatlakozva az érintett számítógépen.
- Ha a számítógép újraindítása nem oldja meg a problémát, kilépése, és csatlakoztassa újra az eszközt az Azure AD. 

**Megjegyzés**: a lépések végrehajtása közben kell lennie a vállalati hálózatban. Lépések nem hajthatók végre, ha nem tud csatlakozni a vállalati infrastruktúra (például utazás közben). 

- Nyisson meg egy emelt szintű parancssort. 
- Nyisson meg egy emelt szintű parancssort, - kattintson a **Start**gombra, kattintson a jobb gombbal a **Parancssor ablakot**, és kattintson a **Futtatás rendszergazdaként**.
- Írja be a *dsregcmd /leave* , majd nyomja le az **ENTER billentyűt**.
- Befejezéskor, írja be a *dsregcmd /join* , és nyomja le az **ENTER billentyűt**.
- Ha elkészült, zárja be a parancssort.
- Indítsa újra a számítógépet, és jelentkezzen be a OneDrive.