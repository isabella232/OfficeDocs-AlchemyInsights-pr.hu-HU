---
title: DLP-szabály nem működik az SSN-hez
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: cfe884a207490a19325ce059652de158c16dc801
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704087"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP kérdések társadalombiztosítási számok

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**DLP-problémák az SSN-ekkel**

Problémái vannak azzal, hogy **az Adatvesztés-megelőzés (DLP)** nem működik a **társadalombiztosítási számot (SSN)** tartalmazó tartalom esetében, amikor bizalmas információtípust használ az Office 365-ben? Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a szükséges információkat, amit a DLP-házirend keres. 
  
Például egy 85%-os megbízhatósági szinttel konfigurált SSN-házirend esetén a rendszer a következőket értékeli ki, és a szabály aktiválásához észlelni kell:
  
- **[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 számjegy, amely formázott vagy formázatlan minta lehet

- **[Minta:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Négy függvény négy különböző mintában keres SSN-eket:

  - Func_ssn a 2011 előtti erős formázású SSN-eket szaggatott vagy szóközzel formázott (ddd-dd-ddd VAGY ddd dddd) formázott ssn-eket keres.

  - Func_unformatted_ssn a 2011 előtti erős formázású SSN-eket kilenc egymást követő számjegyként (dddddddd) formázza.

  - Func_randomized_formatted_ssn 2011 utáni, kötőjelekkel vagy szóközökkel formázott SSN-eket keres (ddd-dd-ddd VAGY ddd dddd)

  - Func_randomized_unformatted_ssn a 2011 utáni SSN-eket kilenc egymást követő számjegyként formázva találja meg (dddddddd)

- **[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nem, nincs Checksum

- **[Meghatározás:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP-házirend 85%-ban biztos abban, hogy az ilyen típusú bizalmas információkat észleli, ha 300 karakteren belül:

  - A [Func_ssn függvény](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) a mintának megfelelő tartalmat talál.

  - A [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) kulcsszó található. Példák a kulcsszavak közé tartozik: *Társadalombiztosítási, Társadalombiztosítási #, Soc Sec, SSN* . Például a következő minta aktiválódik a DLP SSN-házirend: **SSN: 489-36-8350**
  
Ha többet szeretne tudni arról, hogy mi szükséges az SSN-ek észleléséhez a tartalomhoz, olvassa el a cikk következő szakaszát: [A bizalmas információtípusok mit keresnek az SSN-ek számára?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Egy másik beépített bizalmas információtípus használatával a következő cikkben további információt talál arról, hogy mi szükséges más típusokhoz: [Mit keresnek a bizalmas információtípusok?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  