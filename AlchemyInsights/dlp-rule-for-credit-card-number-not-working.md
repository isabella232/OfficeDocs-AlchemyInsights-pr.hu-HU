---
title: Nem működő hitelkártyaszám DLP-szabálya
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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005092"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-problémák hitelkártyaszámokkal

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**DLP-problémák hitelkártyaszámokkal**

Az Adatveszteség-megelőzés **(DLP)** nem működik **olyan** tartalom esetén, amely hitelkártyaszámot tartalmaz, ha bizalmas adatveszteség-megelőzési adattípust használ az O365-ben? Ebben az esetben győződjön meg arról, hogy a tartalom tartalmazza a DLP-házirend kiértékelésekor a szükséges információkat. Egy 85%-os megbízhatósági szinttel konfigurált hitelkártya-házirend esetén például az alábbi feltételeket értékeli ki a rendszer, és a szabály csak akkor aktiválódik, ha észleli őket: 
  
- **[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 számjegy, formázható vagy formázatlan (ddddddd), és át kell adni a Luhn-tesztet.

- **[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Rendkívül összetett és hatékony minta, amely a világ összes jelentős márkajegyének kártyáit észleli, beleértve a Visa, a MasterCard, a Discover Card, a JCB, az American Express, az ajándékkártyákat és a Diner-kártyákat.

- **[Ellenőrzőum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Igen, Luhn-ellenőrzőum

- **[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP-házirend 85%-os magabiztosan észleli ezt a bizalmas információt, ha 300 karakteren belül:

  - A függvény Func_credit_card mintára illeszkedő tartalmat talál.

  - Az alábbiak egyike igaz:

  - Található egy Keyword_cc_verification.

  - Található egy Keyword_cc_name

  - A függvény Func_expiration_date talál egy megfelelő formátumú dátumot.

  - Az ellenőrzőum halad

    Az alábbi példa például DLP-hitelkártyaszám-házirend esetén aktiválódik:

  - Visa: 4485 3647 3952 7352
  
  - Lejár: 2009.02.02.

Ha további információra van szüksége **arról,** hogy mi szükséges ahhoz, hogy a rendszer észlelni tudja a hitelkártyaszámokat a tartalomhoz, tekintse meg a cikk következő szakaszát: A bizalmas adatok típusainak keresve [Hitelkártya#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Más, beépített bizalmas információtípust használva a következő cikkben talál információt a más típusokhoz szükséges információkról: Mit keresnek a bizalmas [adattípusok?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  