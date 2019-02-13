---
title: DLP szabály Nekünk bankszámla száma nem működik
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916418"
---
Hogy problémák adódnak az **Adatok elvesztésének megakadályozása (DLP)** tartalom **USA bankszámla számát** tartalmazó O365 a DLP érzékeny adatok típusa használatakor nem működik? Ha igen, ellenőrizze, hogy a tartalom olvasható Mi a DLP házirendet keres, ha azt értékelje ki a szükséges adatokat. 
  
Például **Amerikai bankszámlaszám** házirend konfigurálva 85 %-os megbízhatósági szint, a következő értékelik, és fel kell deríteni a kiváltó szabály: 
  
- **[Formátuma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 számjegy 
    
- **[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** egymást követő számjegyből álló 8-17. 
    
- **[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nem, nincs nincs ellenőrzőösszeg 
    
- **[Meghatározása:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP házirend abban, hogy ilyen jellegű érzékeny adatokat észlelt 75 %-át Ha a közelség 300 karakter belül: 
    
  - A reguláris kifejezés Regex_usa_bank_account_number tartalom, amely megfelel a minta keresése
    
  - A Keyword_usa_Bank_Account kulcsszó található.
    
    Például, indítsa el a következő minta az **Egyesült Államok bankszámlaszám** házirend: folyószámla 78344011 
    
**USA bankszámla szám** állapítható meg a tartalom szükséges további tájékoztatást a következő részben a cikkben: [Mi az érzékeny adattípusok USA bankszámla szám keresése](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
A beépített érzékeny információk különböző típusú cikke információ szükséges egyéb Újdonságok: [keressen Mi a bizalmas információk típusai](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

