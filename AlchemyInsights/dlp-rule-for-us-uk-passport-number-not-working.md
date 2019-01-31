---
title: DLP szabály az USA / UK útlevél száma nem működik
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 5722f7b6c9a2f905fed2ef4164787e020260edf7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656425"
---
Akkor problémák adódnak az **Adatok elvesztésének megakadályozása (DLP)** tartalmazó tartalom nem működik a **USA / UK útlevél száma** O365 a DLP érzékeny adatok típusa használatakor? Ha igen, ellenőrizze, hogy a tartalom olvasható Mi a DLP házirendet keres, ha azt értékelje ki a szükséges adatokat. 
  
Például, ha egy **US / UK útlevél száma** 75 %-os megbízhatósági szint konfigurált házirend, a következő értékelik, és fel kell deríteni a kiváltó szabály 
  
- **[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Kilenc számjegy 
    
- **[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Kilenc egymást követő számjegyből álló 
    
- **[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nem, nincs nincs ellenőrzőösszeg 
    
- **[Meghatározása:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP házirend abban, hogy ilyen jellegű érzékeny adatokat észlelt 75 %-át Ha a közelség 300 karakter belül: 
    
  - A függvény Func_usa_uk_passport tartalom, amely megfelel a minta keresése.
    
  - A Keyword_passport kulcsszó található.
    
    Például, indítsa el a következő minta esetében a **USA / UK útlevél száma** házirend: 123456789 amerikai útlevél száma 
    
További információt az Egyesült Államok szükséges / UK útlevél száma felismerését a tartalom a következő részben az e cikkben: [Mi a bizalmas információ típusú keresés amerikai / UK útlevél száma](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
A beépített érzékeny információk különböző típusú cikke információ szükséges egyéb Újdonságok: [keressen Mi a bizalmas információk típusai](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

