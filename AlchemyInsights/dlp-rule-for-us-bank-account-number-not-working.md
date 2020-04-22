---
title: DLP-szabály az amerikai bankszámlaszám nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704041"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problémák az amerikai bankszámlaszámokkal

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**DLP-problémák az amerikai bankszámlaszámokkal**

Problémái vannak az **adatveszteség-megelőzéssel (DLP),** amely nem működik **az amerikai bankszámlaszámot** tartalmazó tartalom esetében, amikor Az O365-ben DLP-érzékeny információtípust használ? Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a szükséges információkat, amit a DLP-házirend keres, amikor kiértékeli.
  
A 85%-os megbízhatósági szinttel konfigurált **US Bankszámlaszám-házirend** esetében például a rendszer a következőket értékeli ki, és a szabály aktiválásához észlelni kell:
  
- **[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 számjegy

- **[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 egymást követő számjegy.

- **[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nem, nincs Checksum

- **[Meghatározás:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP-házirend 75%-ban biztos abban, hogy az ilyen típusú bizalmas információkat észleli, ha 300 karakteren belül:

  - A reguláris kifejezés Regex_usa_bank_account_number a mintának megfelelő tartalmat talál

  - A Keyword_usa_Bank_Account kulcsszó található.

    Például a következő minta aktiválódik az **Amerikai Egyesült Államok bankszámlaszám-házirendjének:** 78344011 folyószámla

Ha többet szeretne tudni arról, hogy mi szükséges ahhoz, hogy **egy amerikai bankszámlaszámot** észleljen a tartalomhoz, olvassa el a cikk következő szakaszát: [A bizalmas információtípusok az USA bankszámlaszámát keresik?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Egy másik beépített bizalmas információtípus használatával a következő cikkben további információt talál arról, hogy mi szükséges más típusokhoz: [Mit keresnek a bizalmas információtípusok?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  