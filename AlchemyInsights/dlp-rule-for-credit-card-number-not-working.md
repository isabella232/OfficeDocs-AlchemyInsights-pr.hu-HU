---
title: DLP szabály nem működik a hitelkártya száma
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404500"
---
Az **Adatok elvesztésének megakadályozása (DLP)** nem működik a tartalom egy **Hitelkártya számát** tartalmazó, O365 a DLP érzékeny adatok típusa használatakor problémák lépnek? Ha igen, ellenőrizze, hogy a tartalom tartalmazza az aktiváláshoz szükséges adatokat az a DLP házirendet, amikor azt értékelik. Például **hitelkártya-házirend** konfigurálva 85 %-os megbízhatósági szint, a következő értékelik, és fel kell deríteni a kiváltó szabály: 
  
- **[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 számjegyből állhatnak, amelyek formázhatók vagy formázatlan (dddddddddddddddd), és meg kell felelnie a Luhn. 
    
- **[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Nagyon bonyolult és nagy teljesítményű minta által észlelt minden jelentős márka világszerte, beleértve a Visa, Mastercard, Fedezze fel a kártya, JCB, American Express, ajándékutalványok és diner kártyák kártyáit. 
    
- **[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Igen, a Luhn-ellenőrzőösszeg 
    
- **[Meghatározása:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP házirend abban, hogy ilyen jellegű érzékeny adatokat észlelt 85 % Ha belül a közelében 300 karakter: 
    
  - A függvény Func_credit_card tartalom, amely megfelel a minta keresése.
    
  - A következők egyike igaz: 
    
  - A Keyword_cc_verification kulcsszó található.
    
  - A Keyword_cc_name kulcsszó található.
    
  - A Func_expiration_date függvény dátum megkeresi a megfelelő dátum formátuma.
    
  - Az ellenőrzőösszeg fázisok
    
    Például a következő minta DLP hitelkártya száma házirend megjelenik:
    
  - Vízum: 4485 3647 3952 7352 
    
  - Lejár: 2/2009
    
**Hitelkártya száma** a tartalom felismerését szükséges további tájékoztatást a következő részben a cikkben: [Mi az érzékeny adattípusok keresse meg a hitelkártya száma](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
A beépített érzékeny információk különböző típusú cikke információ szükséges egyéb Újdonságok: [keressen Mi a bizalmas információk típusai](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

