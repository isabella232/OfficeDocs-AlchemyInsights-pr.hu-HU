---
title: Az SSN-re vonatkozó DLP-szabály nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004984"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-problémák a társadalombiztosítási számokkal

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**DLP-problémák az SSN-ekkel**

Nem működik az Adatveszteség-megelőzés **(DLP)** olyan tartalom esetén, amely bizalmas adattípust használ egy társadalombiztosítási számot **(SSN)** tartalmazó Microsoft 365? Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a DLP-házirend tartalmához szükséges információkat. 
  
Egy 85%-os megbízhatósági szinttel konfigurált SSN-házirend esetén például a következőt értékeli ki a rendszer, és a szabály csak akkor aktiválódik, ha észleli őket:
  
- **[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 számjegy, amelyek formázott vagy formázatlan mintában lehetnek

- **[Minta:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Négy függvény az SSN-eket négy különböző mintában keresse:

  - Func_ssn 2011 előtti, kötőjelekkel vagy szóközöket (ddd-dd-dddd VAGY ddd dd dddd) formázott, 2011 előtti SSN-eket talál.

  - Func_unformatted_ssn 2011 előtti, formázatlan, egymást követő kilenc számjegyből álló (dddddddddd) SSN-eket talál.

  - Func_randomized_formatted_ssn 2011 utáni, kötőjelekkel vagy szóközöket (ddd-dd-dddd VAGY ddd dd dddd) formázott SSN-eket is megtalálja.

  - Func_randomized_unformatted_ssn 2011 utáni, kilenc egymást követő számjegyként formázatlan (dddddddddd) SSN-t talál.

- **[Ellenőrzőum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nem, nincs Ellenőrzőum

- **[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP-házirend 85%-os magabiztosan észleli ezt a bizalmas információt, ha 300 karakteren belül:

  - A [függvény Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) mintára illeszkedő tartalmat talál.

  - Található egy [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) Kulcsszavak például a következő:  *Social Security, Social Security#, Soc Sec , SSN*  . A DLP SSN házirendjéből például a következő minta aktiválódik: **SSN: 489-36-8350**
  
A tartalomhoz szükséges SSN-ek észleléséhez további információt a jelen cikk következő szakaszában talál: A bizalmas adattípusok által keresve az [SSN-ek](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Más, beépített bizalmas információtípust használva a következő cikkben talál információt a más típusokhoz szükséges információkról: Mit keresnek a bizalmas [adattípusok?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  