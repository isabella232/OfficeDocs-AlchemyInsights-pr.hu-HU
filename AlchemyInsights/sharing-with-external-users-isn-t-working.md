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
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747600"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>A SharePoint-tartalom megosztása a külső felhasználók problémák megoldása

Ellenőrizze, hogy a szervezet külső megosztás van kapcsolva:
  
1. Keresse fel a [szolgáltatások &amp; -bővítmények a Microsoft 365 felügyeleti központ lapján](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), majd a **helyek**gombra.
    
2. Győződjön meg arról, hogy a beállítás be van kapcsolva, "On." Ha be van jelölve "Csak meglévő külső felhasználók", ellenőrizze, hogy a külső felhasználói a Microsoft 365 felügyeleti központ szerepel.
    
Ellenőrizze, hogy a webhely kapcsolva külső megosztás. Klasszikus helycsoport:
  
1. Az új SharePoint felügyeleti központ bal oldali ablaktáblájában kattintson a **helyek**gombra.
    
2. Jelölje ki a hely vagy helyek, és a menüszalagon kattintson a **megosztás**parancsra.
    
Az Office 365 csoporthoz tartozó csoportwebhelyet, vagy kommunikációs hely:
  
- Új webhely típusaival rendelkezik az azonos megosztási beállítása a szervezeti szintű beállítás, kivéve, ha a szervezeti szintű beállítás lehetővé teszi, hogy nem szükséges bejelentkezési hivatkozásokra fájlok megosztása. Ebben az esetben a webhelyek új és meglévő külső felhasználók bejelentkezés megosztás engedélyezése. Bizonyos webhelyek módosításához használja az új SharePoint-felügyeleti központ vagy PowerShell. [További információ](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> A külső webhelyek megosztási beállítása lehet szigorúbb, mint a szervezeti szintű beállítást, de nem több mint a szervezeti szintű beállítás alkalmazásszolgáltatásokra. 
  

