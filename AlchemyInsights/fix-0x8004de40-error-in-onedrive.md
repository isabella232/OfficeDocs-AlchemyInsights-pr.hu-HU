---
title: A 0x8004de40 kijavítva a OneDrive-ban
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649750"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>A 0x8004de40 kijavítva a OneDrive-ban

Ha Windows 7 rendszert használ, és ez a hibaüzenet jelenik meg, a Frissítés az alapértelmezett biztonságos protokollként való [TLS 1.1 és TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)engedélyezéséhez a Windows rendszerbenHTTP.

Ha Windows 10 rendszert futtat, és egy hibaüzenet 0x8004de40 OneDrive-val:

- Indítsa újra az érintett számítógépet, miközben az Acitve-címtár tartományához csatlakozik.
- Ha egy újraindítás nem oldja meg a problémát, oldja fel az eszközhöz való, majd az Azure AD-ból való újracsatlakozáskor. 

**Megjegyzés:** A lépések végrehajtása közben a vállalati hálózatnak kell lennie. Ne hajtsa végre ezeket a lépéseket, ha nem csatlakozik vállalati infrastruktúrához (például utazás közben). 

1. Nyisson meg egy rendszergazdai jogú parancssort a **Start** menüből, kattintson a jobb gombbal a **Parancssor** elemre, majd válassza a **Futtatás rendszergazdaként parancsot.**

1. Írja *be a dsregcmd /leave parancsot, és* nyomja le az Enter **billentyűt.**

1. Ha elkészült, írja be a *dsregcmd /join parancsot,* és nyomja le az **Enter billentyűt.**

1. Ha elkészült, zárja be a parancssort.

1. Indítsa újra a számítógépet, és jelentkezzen be a OneDrive-ba.