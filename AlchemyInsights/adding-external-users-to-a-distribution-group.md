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
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663515"
---
# <a name="add-external-users-to-a-distribution-group"></a>Külső felhasználók felvétele terjesztési csoportba

Külső partnerek felvétele egy terjesztési csoportba (DG) két lépésből álló folyamat:
  
1. Levelezési névjegykártya létrehozása külső felhasználó számára:
    
    1. A felügyeleti központban lépjen a **felhasználók**  >  [partnerek](https://admin.microsoft.com/adminportal/home#/Contact) lapjára. 
    
    2. Jelölje be **a névjegykártya felvétele**jelölőnégyzetet.
    
    3. Adja meg a névjegy adatait, és válassza a **Hozzáadás**gombot.
    
2. Adja hozzá a levelezési ügyfelet a DG-hoz:
    
    1. A felügyeleti központban lépjen a **csoportok**  >  [csoportjai](https://admin.microsoft.com/adminportal/home#/groups) lapra. 
    
    2. Keresse meg azt a Főigazgatóságot, amelyhez hozzá szeretné adni a külső felhasználót, és a Szerkesztés párbeszédpanel megnyitásához jelölje ki azt.
    
    3. A **tagok** lapon válassza az **összes megtekintése és a tagok kezelése**lehetőséget. 
    
    4. Válassza a **Tagok hozzáadása**lehetőséget.
    
    5. Jelölje ki az előző lépésben létrehozott levelezési névjegykártyát, és válassza a **Mentés**gombot.
    
Ha az alábbi lépéseket követve a külső felhasználók nem tudnak e-maileket küldeni a DG-nek, vagy nem érkeznek meg az e-mailek, akkor lehet, hogy a DG csak a belső felhasználóktól érkező e-mailek engedélyezésére van megjelölve. Ezt a konfigurációt követve ellenőrizheti az [itt](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)leírt útmutatást.
  
 **Megjegyzés:** Ezek az utasítások nem érvényesek, ha a csoport típusa "Microsoft 365 Group" a "terjesztési csoport" helyett. Ebben az esetben a külső felhasználót közvetlenül a csoportba veheti fel az Outlookból. A cikkben részletes információkat talál a Microsoft 365-csoportok vendégeinek, valamint a külső vendégek hozzáadásának lépéseit ismertető [cikkben](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  