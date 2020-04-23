---
title: 0x8004de40 hiba javítása a OneDrive-on
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716030"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>0x8004de40 hiba javítása a OneDrive-on

Ha 0x8004de40-es hibaüzenet jelenik meg a OneDrive-val:

- Indítsa újra az érintett számítógépet, miközben az Acitve Directory tartományhoz csatlakozik.
- Ha egy újraindítás nem oldja meg a problémát, válassza le, és csatlakozzon újra az eszközhöz az Azure AD-ből. 

**Megjegyzés:** A lépések végrehajtása közben a vállalati hálózaton kell lennie. Ne hajtsa végre ezeket a lépéseket, ha nem tud csatlakozni a vállalati infrastruktúrához (például utazás közben). 

- Nyisson meg egy rendszergazda jogú parancssort. 
- Emelt szintű parancssor megnyitásához kattintson a - **Start**gombra, kattintson a jobb gombbal **a Parancssor parancsra,** majd kattintson a **Futtatás rendszergazdaként parancsra.**
- Írja be *a dsregcmd /leave kapcsolót,* és nyomja **le az Enter billentyűt.**
- Ha kész, írja be *a dsregcmd /join kapcsolót,* és nyomja **le az Enter billentyűt.**
- Ha befejeződött, zárja be a parancssort.
- Indítsa újra a számítógépet, és jelentkezzen be a OneDrive-ba.