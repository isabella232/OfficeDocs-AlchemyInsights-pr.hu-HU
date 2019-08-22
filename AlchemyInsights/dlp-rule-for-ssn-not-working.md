---
title: DLP szabály a TAJ-szám nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529858"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Társadalombiztosítási számok DLP problémái

Hogy problémák adódnak az **Adatok elvesztésének megakadályozása (DLP)** tartalom a **Társadalombiztosítási szám (SSN)** tartalmazó, a bizalmas adatok típusa használatakor az Office 365 rendszerben nem működik? Ha igen, ellenőrizze, hogy a tartalom a DLP politika feladata a szükséges adatokat tartalmazza. 
  
Például a TAJ-szám házirend konfigurálva 85 %-os megbízhatósági szint, a következő értékelik, és fel kell deríteni a kiváltó szabály:
  
- **[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 számjegy, esetleg egy formázott vagy nem formázott minta

- **[Minta:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** A négy különböző mintázatú SSNs négy függvény keresése:

  - Func_ssn SSNs pre-2011 erős formátummal formázott kötőjeleket és szóközöket (nnn-nn-nnnn vagy ddd nn dddd) talál.

  - Func_unformatted_ssn SSNs pre-2011 erős formázással, amelyek nem formázott, kilenc egymást követő számjegyből (ddddddddd) talál.

  - Func_randomized_formatted_ssn megtalálja a post-2011 SSNs formázott kötőjeleket és szóközöket (nnn-nn-nnnn vagy ddd nn dddd)

  - Func_randomized_unformatted_ssn megtalálja a post-2011 SSNs, amelyek nem formázott, kilenc egymást követő számjegyből (ddddddddd)

- **[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nem, nincs nincs ellenőrzőösszeg

- **[Meghatározása:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP házirend abban, hogy ilyen jellegű érzékeny adatokat észlelt 85 % Ha belül a közelében 300 karakter:

  - A [függvény Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) tartalom, amely megfelel a minta keresése.

  - A [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) kulcsszó található. Példák a kulcsszavakat tartalmazza: *társadalombiztosítási, társadalombiztosítási #, Soc (mp), a TAJ-szám* . Például a TAJ-szám DLP házirend megjelenik a következő minta: **Taj-szám: 489-36-8350**
  
Mi az SSNs a tartalom kimutatásához szükséges további tájékoztatást a következő részben a cikkben: [Mi az érzékeny adattípusok SSNs keresése](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
A beépített érzékeny információk különböző típusú cikke információ szükséges egyéb Újdonságok: [keressen Mi a bizalmas információk típusai](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  