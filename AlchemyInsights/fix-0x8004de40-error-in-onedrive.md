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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525061"
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