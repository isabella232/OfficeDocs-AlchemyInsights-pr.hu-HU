---
title: A 0x8004de40 hibáinak elhárítása a OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745132"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>A 0x8004de40 hibáinak elhárítása a OneDrive

Ha a OneDrive-0x8004de40 hibaüzenetet kap:

- Indítsa újra az érintett számítógépet, miközben csatlakozik a Acitve-címtár tartományához.
- Ha az újraindítás nem oldja meg a problémát, akkor csatlakozzon az Azure AD-hoz, és csatlakozzon újra az eszközhöz. 

**Megjegyzés**: a lépések végrehajtása közben a vállalati hálózaton kell lennie. Ne végezze el ezeket a lépéseket, ha nem tud csatlakozni a vállalati infrastruktúrához (például utazás közben). 

- Nyisson meg egy rendszergazdai jogú parancssort. 
- Ha meg szeretne nyitni egy rendszergazdai jogú parancssort, kattintson a **Start**gombra, kattintson a jobb gombbal a parancssor elemre, és válassza **a Futtatás rendszergazdaként** **parancsot**.
- Írja be a *dsregcmd/Leave* , és nyomja le az **entert**.
- Ha elkészült, írja be a *dsregcmd/JOIN* , és nyomja le az **ENTER**billentyűt.
- Ha elkészült, zárja be a parancssort.
- Indítsa újra a számítógépet, és jelentkezzen be a OneDrive.