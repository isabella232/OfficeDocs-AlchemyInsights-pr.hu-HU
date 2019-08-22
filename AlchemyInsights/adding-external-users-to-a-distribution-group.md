---
title: Terjesztési csoport külső felhasználó hozzáadása
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494529"
---
# <a name="add-external-users-to-a-distribution-group"></a>Külső felhasználók hozzáadása a terjesztési csoportot?

Hozzáadása egy külső partner, a terjesztési csoport (DG) egy 2 lépésből álló folyamat:
  
1. A külső felhasználó levelezési névjegy létrehozása:
    
    1. A felügyeleti központ, keresse meg a **felhasználók** > [Névjegyalbum](https://admin.microsoft.com/adminportal/home#/Contact) lapon. 
    
    2. Válassza ki a **Partner felvétele**.
    
    3. Írja be a partner adatait, és válassza a **Hozzáadás gombra**.
    
2. Adja hozzá a levél az ügyfélnek a DG:
    
    1. A **csoportok**Ugrás az admin center > [csoportok](https://admin.microsoft.com/adminportal/home#/groups) lapon. 
    
    2. Keresse meg a DG szeretne hozzáadni a külső felhasználó, és jelölje ki azt a Szerkesztés párbeszédpanel megnyitásához.
    
    3. A **tagok** lapon jelölje be **az összes megtekintése és kezelése a tagok**. 
    
    4. Válassza ki a **Tagok hozzáadása**.
    
    5. Válassza ki az előző lépésben létrehozott levelezési ügyfelet, és válassza a **Mentés**.
    
Ha ezen lépések után a külső felhasználók nem küldhet e-maileket a DG, vagy nem kap e-mailek belőle, lehet, hogy a DG e-mailek engedélyezése csak a belső felhasználók számára van megjelölve. Ellenőrizze a konfigurációt, és javítsa ki a következő utasításokat [Itt](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).
  
 **Megjegyzés:** Ezeket az utasításokat nem alkalmazhatók, ha a csoport típusa "Office 365-csoport" helyett "Terjesztési csoport." Ha ez az eset, hozzáadhatja a külső felhasználó közvetlenül a csoport az Outlook programból. Office 365 csoportok vendégek részletes tájékoztatást és utasításokat külső Vendégek hozzáadása a [cikkben](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)található.
  