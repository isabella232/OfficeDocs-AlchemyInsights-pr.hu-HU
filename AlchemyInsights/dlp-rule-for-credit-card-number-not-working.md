---
title: Nem működött a hitelkártya-számhoz tartozó DLP-szabály
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679443"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problémák a hitelkártya-számokkal

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**DLP-problémák a hitelkártya-számokkal**

Problémát tapasztal az **adatvesztés-megelőzéssel (DLP)** kapcsolatban, ha nem működik a **hitelkártyát** tartalmazó tartalom, ha a O365-ban DLP típusú bizalmas adattípust használ? Ha igen, gondoskodjon arról, hogy a tartalom a kiértékeléskor a DLP-házirend elindításához szükséges információkat tartalmazza. A 85%-os megbízhatósági szinttel konfigurált **hitelkártya-házirend** esetén például a program kiértékeli az alábbiakat, és a következőhöz kell észlelni:
  
- **[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 számjegy, amely formázható vagy formázható (közönséges számsorozatként), és meg kell adnia a Luhn tesztet.

- **[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Nagyon bonyolult és robusztus minta, amely az egész világon elérhető főbb márkák kártyáit észleli, többek között Visa, MasterCard, Discover Card, JCB, American Express, Gift Cards és Diner kártyával.

- **[Ellenőrzőösszeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Igen, az Luhn ellenőrzőösszeg

- **[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP-házirend 85%-os megbízhatósági szinttel jelenti az ilyen típusú bizalmas adatok észlelését, ha az 300 karaktereken belül:

  - A függvény Func_credit_card megkeresi a mintázattal egyező tartalmat.

  - Az alábbiak egyike igaz:

  - A Keyword_cc_verification kulcsszója megtalálható.

  - Keyword_cc_name található kulcsszó

  - A függvény Func_expiration_date a megfelelő dátum formátumban keresi a dátumot.

  - Az ellenőrzőösszeg áthalad

    Az alábbi példa például egy DLP-beli hitelkártya-házirendet indít el:

  - Visa: 4485 3647 3952 7352
  
  - Lejárat: 2/2009

Ha többet szeretne megtudni arról, hogy mire van szüksége a tartalomhoz a **hitelkártyaszám** felderítéséhez, olvassa el a következő cikket: [Mi a bizalmas adattípusok keresése a hitelkártyával #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Ha más beépített bizalmas adattípust használ, további információt a következő témakörben talál: [a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  