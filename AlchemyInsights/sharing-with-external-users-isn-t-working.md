---
title: A külső felhasználók megosztása nem működik
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207687"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>A SharePoint-tartalom megosztása a külső felhasználók problémák megoldása

Ellenőrizze, hogy a szervezet külső megosztás van kapcsolva:
  
1. Keresse fel a [szolgáltatások &amp; -bővítmények a Microsoft 365 felügyeleti központ lapján](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), majd a **helyek**gombra.
    
2. Győződjön meg arról, hogy a beállítás be van kapcsolva, "On." Ha be van jelölve "Csak meglévő külső felhasználók", ellenőrizze, hogy a külső felhasználói a Microsoft 365 felügyeleti központ szerepel.
    
Ellenőrizze, hogy a webhely kapcsolva külső megosztás. Klasszikus helycsoport:
  
1. A klasszikus SharePoint felügyeleti központ bal oldali ablaktáblájában kattintson a **webhelycsoportok**.
    
2. Jelölje ki a hely vagy helyek, és a menüszalagon kattintson a **megosztás**parancsra.
    
Az Office 365 csoporthoz tartozó csoportwebhelyet, vagy kommunikációs hely:
  
- Új webhely típusaival rendelkezik az azonos megosztási beállítása a szervezeti szintű beállítás, kivéve, ha a szervezeti szintű beállítás lehetővé teszi, hogy nem szükséges bejelentkezési hivatkozásokra fájlok megosztása. Ebben az esetben a webhelyek új és meglévő külső felhasználók bejelentkezés megosztás engedélyezése. Az új SharePoint felügyeleti központ (kép) vagy a PowerShell segítségével bizonyos webhelyek módosításához. [Tudjon meg többet](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> A külső webhelyek megosztási beállítása lehet szigorúbb, mint a szervezeti szintű beállítást, de nem több mint a szervezeti szintű beállítás alkalmazásszolgáltatásokra. 
  

