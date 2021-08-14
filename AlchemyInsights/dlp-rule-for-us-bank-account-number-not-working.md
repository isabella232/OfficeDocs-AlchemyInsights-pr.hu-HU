---
title: Nem működik az US bankfiókszámra vonatkozó DLP-szabály
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
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005020"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-problémák az amerikai bankszámlaszámokkal

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**DLP-problémák az amerikai bankszámlaszámokkal**

Az Adatveszteség-megelőzés **(DLP)** nem működik olyan tartalom esetén, amely us **bankfiókszámot** tartalmaz, ha bizalmas DLP-adattípust használ az O365-ben? Ebben az esetben győződjön meg arról, hogy a tartalom tartalmazza azokat az információkat, amelyekre a DLP-házirend értékelésekor szüksége van.
  
Egy 85%-os megbízhatósági szinttel konfigurált us bankfiókszám-házirend esetén például a következőt értékeli ki a rendszer, és a szabály csak akkor aktiválódik, ha: 
  
- **[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 számjegy

- **[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8–17 egymást követő számjegy.

- **[Ellenőrzőum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nem, nincs Ellenőrzőum

- **[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP-házirend 75%-os magabiztosan észleli ezt a típusú bizalmas információt, ha 300 karakteren belül:

  - A reguláris Regex_usa_bank_account_number mintára illeszkedő tartalmat talál.

  - Található egy Keyword_usa_Bank_Account.

    Az amerikai bankszámlaszám házirend esetében például **az** alábbi minta aktiválódik: Checking Account 78344011

Ha további információra van szüksége **arról,** hogy mi szükséges ahhoz, hogy a rendszer észlelni tudja az egyesültünki bankszámlaszámokat a tartalomhoz, tekintse meg a jelen cikk következő [szakaszát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) Az amerikai bankszámlaszámok bizalmas adattípusa
  
Más, beépített bizalmas információtípust használva a következő cikkben talál információt a más típusokhoz szükséges információkról: Mit keresnek a bizalmas [adattípusok?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  