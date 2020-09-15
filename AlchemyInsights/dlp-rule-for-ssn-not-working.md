---
title: Nem működött a SSN szabály
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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679371"
---
# <a name="dlp-issues-with-social-security-numbers"></a>A társadalombiztosítási számokkal kapcsolatos DLP-problémák

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**DLP-problémák a azonosítókat keresi.-ban**

Problémát tapasztal az **adatvesztés-megelőzéssel (DLP)** kapcsolatban, ha nem működik a **társadalombiztosítási szám (SSN)** tartalmú tartalom a Microsoft 365 bizalmas adattípusa használatakor? Ha igen, győződjön meg arról, hogy a tartalom a DLP-házirend kinézetéhez szükséges információkat tartalmazza. 
  
Egy 85%-os megbízhatósági szinttel konfigurált SSN-házirend esetében például a program kiértékeli a következőt, és a következőhöz kell észlelni:
  
- **[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 számjegy, amelyek formázott vagy formázatlan mintázatként jelenhetnek meg

- **[Minta:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Négy függvény a azonosítókat keresi. keres négy különböző mintázatban:

  - A Func_ssn megkeresi a 2011-os erős formázást, amely szaggatott vagy szóköz formátumú (DDD-dd-azonosítókat keresi. vagy DDD dd-vel) van formázva.

  - A Func_unformatted_ssn olyan erős formázással 2011 rendelkező azonosítókat keresi. keres, amelyek nem formázottak kilenc egymást követő számjegyként (ddddddddd)

  - A Func_randomized_formatted_ssn a gondolatjelekkel vagy szóközökkel formázott 2011-azonosítókat keresi. (DDD-DD-vagy DDD dd)

  - A Func_randomized_unformatted_ssn megkeresi a 2011 azonosítókat keresi., amelyek nem formázottak kilenc egymást követő számjegyet (ddddddddd)

- **[Ellenőrzőösszeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nem, nincs ellenőrzőösszeg

- **[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP-házirend 85%-os megbízhatósági szinttel jelenti az ilyen típusú bizalmas adatok észlelését, ha az 300 karaktereken belül:

  - A [függvény Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) megkeresi a mintázattal egyező tartalmat.

  - A [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) kulcsszója megtalálható. A kulcsszavak példái a következők:  *társadalombiztosítási, társadalombiztosítási #, SoC sec, SSN*  . Az alábbi példa például a DLP SSN-házirendet eredményezte: **ssn: 489-36-8350**
  
Ha további információra van szüksége a azonosítókat keresi. a tartalomhoz való észleléséhez, olvassa el a jelen cikk következő szakaszát: [Mi a bizalmas adattípusok keresése a azonosítókat keresi.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) -ban
  
Ha más beépített bizalmas adattípust használ, további információt a következő témakörben talál: [a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  