---
title: DLP szabály nem működik a hitelkártya száma
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389579"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problémáinak hitelkártyaszámok

Az **Adatok elvesztésének megakadályozása (DLP)** nem működik a tartalom egy **Hitelkártya számát** tartalmazó, O365 a DLP érzékeny adatok típusa használatakor problémák lépnek? Ha igen, ellenőrizze, hogy a tartalom tartalmazza az aktiváláshoz szükséges adatokat az a DLP házirendet, amikor azt értékelik. Például **hitelkártya-házirend** konfigurálva 85 %-os megbízhatósági szint, a következő értékelik, és fel kell deríteni a kiváltó szabály:
  
- **[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 számjegyből állhatnak, amelyek formázhatók vagy formázatlan (dddddddddddddddd), és meg kell felelnie a Luhn.

- **[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Nagyon bonyolult és nagy teljesítményű minta által észlelt minden jelentős márka világszerte, beleértve a Visa, MasterCard, Fedezze fel a kártya, JCB, American Express, ajándékutalványok és diner kártyák kártyáit.

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
  