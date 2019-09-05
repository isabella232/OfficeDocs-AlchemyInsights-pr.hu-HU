---
title: Külső felhasználók hozzáadása a terjesztési csoporthoz
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737875"
---
# <a name="add-external-users-to-a-distribution-group"></a>Külső felhasználók hozzáadása terjesztési csoporthoz

A terjesztési csoporthoz (DG) külső kapcsolattartó hozzáadása két lépésben történik:
  
1. Levelezési kapcsolat létrehozása a külső felhasználó számára:
    
    1. Az admin központban lépjen a **felhasználók** > [névjegyalbumoldalára](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Válassza **a Névjegy hozzáadása**-t.
    
    3. Írja be a névjegyhez tartozó adatokat, és válassza a **hozzáad**-t.
    
2. A levelezési kapcsolat felvétele a FŐIGAZGATÓSÁGBA:
    
    1. Az admin központban lépjen a **csoportok** > [csoportjai](https://admin.microsoft.com/adminportal/home#/groups) oldalra. 
    
    2. Keresse meg azt a FŐIGAZGATÓSÁGOT, amelyhez hozzá szeretné adni a külső felhasználót, majd jelölje ki a szerkesztési párbeszédpanel megnyitásához.
    
    3. A **tagok** lapon jelölje be az **összes megtekintése és a tagok kezelése**választógombot. 
    
    4. Válassza a **Tagok felvétele**-t.
    
    5. Válassza ki az előző lépésben létrehozott levelezési névjegyet, majd válassza a **Mentés**-t.
    
Ha a következő lépések megtételét követően a külső felhasználók nem tudnak e-maileket küldeni a DG-nek, vagy nem kapnak e-maileket, akkor lehet, hogy a FŐIGAZGATÓSÁGNAK csak belső felhasználóktól származó leveleket enged meg. Tudod ellenőriz ez alakzat és erősít ez alábbiak a utasítások [itt](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Megjegyzés:** Ezek az utasítások nem alkalmazhatók, ha a csoport típusa "terjesztési csoport" helyett "Office 365 csoport". Ebben az esetben a külső felhasználót közvetlenül is hozzáadhatja a csoporthoz az Outlook programból. Részletes információ az Office 365 csoportokról, a vendégek és a külső vendégek hozzáadására vonatkozó utasítások megtalálhatók [ebben a cikkben](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  