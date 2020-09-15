---
title: Az amerikai bankszámlaszám nem mûködõ DLP-szabály
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679298"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problémák az amerikai bankszámlák számaival

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**DLP-problémák az amerikai bankszámlák számaival**

Problémákat tapasztal az **adatvesztés-megelőzéssel (DLP)** , ha nem működik az **amerikai bankszámlaszám** tartalmazó tartalmaknál a O365-ban DLP típusú bizalmas adattípus használatakor? Ha igen, győződjön meg arról, hogy a tartalom a kiértékeléskor a DLP-házirend szempontjából szükséges információkat tartalmazza.
  
Például az 85%-os megbízhatósági szinttel konfigurált **amerikai bankszámlaszám** -házirend esetén a program kiértékeli az alábbiakat, és a szabálynak a következőképpen kell kiértékelést végeznie:
  
- **[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 számjegyek

- **[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 egymást követő számjegyek.

- **[Ellenőrzőösszeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nem, nincs ellenőrzőösszeg

- **[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP-házirend 75%-os megbízhatósági szinttel jelenti az ilyen típusú bizalmas adatok észlelését, ha az 300 karaktereken belül:

  - A normál kifejezés Regex_usa_bank_account_number megkeresi a mintázatnak megfelelő tartalmat

  - A Keyword_usa_Bank_Account kulcsszója megtalálható.

    A következő minta például az **amerikai bankszámlaszám** -házirend: a 78344011 fiók ellenőrzése

Ha szeretne többet megtudni arról, hogy mire van szükség egy **amerikai bankszámlaszám** a tartalomhoz való felderítéséhez, olvassa el a jelen cikk következő szakaszát: [Mi a bizalmas adattípusok keresése az amerikai bankszámlák számát](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Ha más beépített bizalmas adattípust használ, további információt a következő témakörben talál: [a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  