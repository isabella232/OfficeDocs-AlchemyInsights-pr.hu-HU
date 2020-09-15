---
title: Nem működött a külső felhasználókkal való megosztás
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
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691577"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>SharePoint-tartalmak külső felhasználókkal való megosztásával kapcsolatos problémák megoldása

Győződjön meg arról, hogy a külső megosztás be van kapcsolva a szervezetben:
  
1. Nyissa meg a [szolgáltatások &amp; bővítmények lapot a Microsoft 365 felügyeleti központban](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), és kattintson a **webhelyek**elemre.
    
2. Győződjön meg arról, hogy a beállítás be van kapcsolva. Ha a "csak a meglévő külső felhasználók" beállítás van kiválasztva, győződjön meg arról, hogy a külső felhasználó szerepel a Microsoft 365 felügyeleti központban.
    
Ellenőrizze, hogy be van-e kapcsolva a külső megosztás a webhelyen. Klasszikus webhelycsoport esetén:
  
1. Az új SharePoint felügyeleti központ bal oldali ablaktábláján kattintson a **webhelyek**elemre.
    
2. Jelölje ki a webhelyet vagy a webhelyeket, és kattintson a menüszalag **megosztás**gombjára.
    
Microsoft 365-csoportba tartozó csoportwebhely vagy kommunikációs webhely esetén:
  
- Ezek az új tartalomtípusok ugyanazzal a megosztási beállítással rendelkeznek, mint a szervezeti szintű beállítás, kivéve ha a szervezeti szintű beállítás lehetővé teszi a fájlok megosztását a bejelentkezést nem igénylő hivatkozásokkal. Ebben az esetben a webhelyek lehetővé teszik a megosztást az új és a meglévő külső felhasználókkal, akik bejelentkeznek. Ha módosítani szeretné bizonyos webhelyek beállítását, használja az új SharePoint felügyeleti központot vagy a PowerShellt. [További információ](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> A webhelyek külső megosztási beállítása több korlátozást tartalmazhat, mint a szervezeti szintű beállítás, de nem több megengedhető érték, mint a szervezeti szintű beállítás. 
  

