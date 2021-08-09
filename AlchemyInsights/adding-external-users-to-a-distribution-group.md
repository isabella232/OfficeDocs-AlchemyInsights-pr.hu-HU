---
title: Külső felhasználók felvétele terjesztési csoportba
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934835"
---
# <a name="add-external-users-to-a-distribution-group"></a>Külső felhasználók felvétele terjesztési csoportba

Külső partner terjesztési csoportba való felvétele két lépésből áll:
  
1. Levelezési partner létrehozása a külső felhasználó számára:
    
    1. A felügyeleti központban válassza a Felhasználók  >  [névjegyalbuma lapot.](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Válassza **a Partner felvétele lehetőséget.**
    
    3. Írja be a partner adatait, és válassza a **Hozzáadás gombot.**
    
2. Vegye fel a levelezési partnert a partneri fiókba:
    
    1. A felügyeleti központban kattintson a **Csoportok**  >  [lapra.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Keresse meg azt a csoportot, amelybe fel szeretné vegye a külső felhasználót, és válassza ki, és nyissa meg a szerkesztési párbeszédpanelt.
    
    3. A Tagok **lapon** válassza Az összes megtekintése és a tagok **kezelése lehetőséget.** 
    
    4. Válassza a **Tagok hozzáadása lehetőséget.**
    
    5. Jelölje ki az előző lépésben létrehozott levelezési partnert, és válassza a Mentés **gombot.**
    
Ha a fenti lépések után a külső felhasználók nem tudnak e-maileket küldeni a csoportnak, vagy nem fogadhatnak róla e-maileket, akkor lehet, hogy a csoport úgy van bejelölve, hogy csak a belső felhasználóktól származó e-maileket engedélyezze. Ezt a konfigurációt az itt útmutatást követően ellenőrizheti és [kijavíthatja.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Megjegyzés:** Ezek az utasítások nem érvényesek, ha a csoport típusa "Microsoft 365" a "Terjesztési csoport" helyett. Ebben az esetben a külső felhasználót közvetlenül a csoporthoz használhatja a Outlook. A csoportok Microsoft 365 és a külső vendégek felvételének utasításait ebben a cikkben [olvashatja.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  