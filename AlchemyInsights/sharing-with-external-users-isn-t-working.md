---
title: Nem működik a külső felhasználókkal való megosztás
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304371"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>A külső felhasználókkal SharePoint tartalommegosztási problémák megoldása

Győződjön meg arról, hogy a külső megosztás be van kapcsolva a szervezetében:
  
1. A lap [Szolgáltatások &amp; bővítményeinek](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)lapján kattintson a Microsoft 365 Felügyeleti központ , majd a **Webhelyek elemre.**
    
2. Győződjön meg arról, hogy a beállítás "Be" beállításra van kapcsolva. Ha a "Csak a meglévő külső felhasználók" beállítás van kiválasztva, győződjön meg arról, hogy a külső felhasználó szerepel a Microsoft 365 Felügyeleti központ.
    
Győződjön meg arról, hogy a külső megosztás be van kapcsolva a webhelyen. Klasszikus webhelycsoporthoz:
  
1. Az új felügyeleti SharePoint bal oldali ablaktábláján kattintson a webhelyek **elemre.**
    
2. Jelölje ki a webhelyet vagy webhelyeket, és a menüszalagon kattintson a Megosztás **elemre.**
    
Olyan csapatwebhelyen, amely egy csoport Microsoft 365 kommunikációs webhelyhez tartozik:
  
- Az új webhelytípusok megosztási beállítása megegyezik a szervezeti szintű beállítással, hacsak a szervezeti szintű beállítás nem teszi lehetővé a fájlok bejelentkezést nem igénylő hivatkozásokkal való megosztását. Ebben az esetben a webhelyek lehetővé teszik a megosztást az új és a már bejelentkező külső felhasználókkal. Ha módosítania kell bizonyos webhelyek beállítását, használja az SharePoint felügyeleti központot vagy a PowerShellt. [További információ](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Megjegyzés:** Bármely webhely külső megosztási beállítása lehet szigorúbb, mint a szervezetre vonatkozó beállítás, de nem lehet megengedőbb, mint a szervezetre vonatkozó beállítás. 
  

