---
title: DLP-szabály a hitelkártyaszám nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507408"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problémák hitelkártyaszámokkal

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**DLP-problémák hitelkártyaszámokkal**

Problémái vannak azzal, hogy **az Adatveszteség-megelőzés (DLP)** nem működik a **hitelkártyaszámot** tartalmazó tartalom esetében, amikor Az O365-ben DLP-érzékeny információtípust használ? Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a szükséges információkat a DLP-házirend aktiválásához a kiértékeléskor. A 85%-os megbízhatósági szinttel konfigurált **hitelkártya-házirendek** esetében például a rendszer a következőket értékeli ki, és a szabály aktiválásához észlelni kell őket:
  
- **[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 számjegy, amely formázható vagy formázható (dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd

- **[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Nagyon összetett és robusztus minta, amely észleli a világ összes jelentős márkájának kártyáit, beleértve a Visa, MasterCard, Discover Card, JCB, American Express, ajándékkártyákat és étkezőkártyákat.

- **[Ellenőrző összeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Igen, a Luhn ellenőrző összeg

- **[Meghatározás:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP-házirend 85%-ban biztos abban, hogy az ilyen típusú bizalmas információkat észleli, ha 300 karakteren belül:

  - A Func_credit_card függvény a mintának megfelelő tartalmat talál.

  - Az alábbiak egyike igaz:

  - A Keyword_cc_verification kulcsszó található.

  - A Keyword_cc_name kulcsszó található

  - A Func_expiration_date függvény a megfelelő dátumformátumban keresi a dátumot.

  - Az ellenőrző összeg átmegy

    Például a következő minta a DLP hitelkártyaszám-házirendjének aktiválásához lépki:

  - Vízum: 4485 3647 3952 7352
  
  - Lejár: 2/2009

Ha többet szeretne tudni arról, hogy mi szükséges a **hitelkártyaszám** észleléséhez a tartalomhoz, olvassa el a cikk következő szakaszát: [Milyen bizalmas információtípusok keresnek hitelkártyát#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Egy másik beépített bizalmas információtípus használatával a következő cikkben további információt talál arról, hogy mi szükséges más típusokhoz: [Mit keresnek a bizalmas információtípusok?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  