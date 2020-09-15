---
title: Az Amerikai Egyesült államokbeli Passport-szám nem működött a DLP-szabály szerint
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679226"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>A DLP-US/UK-hu/UK Passport-számokkal kapcsolatos problémák

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**DLP-problémák az Amerikai Egyesült államokbeli Passport-számokkal**

Problémákat tapasztal az **adatvesztés-megelőzéssel (DLP)** , ha nem működik az **amerikai/brit útlevél számát** tartalmazó tartalom, ha a O365-ban DLP típusú bizalmas adattípust használ? Ha igen, győződjön meg arról, hogy a tartalom a kiértékeléskor a DLP-házirend szempontjából szükséges információkat tartalmazza.
  
Például az 75%-os megbízhatósági szinttel konfigurált **amerikai/brit Passport** -házirend esetén a program kiértékeli az alábbiakat, és észleli a szabályt az indításhoz.
  
- **[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Kilenc számjegy

- **[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Kilenc egymást követő számjegy

- **[Ellenőrzőösszeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nem, nincs ellenőrzőösszeg

- **[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP-házirend 75%-os megbízhatósági szinttel jelenti az ilyen típusú bizalmas adatok észlelését, ha az 300 karaktereken belül:

  - A függvény Func_usa_uk_passport megkeresi a mintázattal egyező tartalmat.

  - A Keyword_passport kulcsszója megtalálható.

    Az alábbi minta például az Amerikai Egyesült államokbeli **Passport-számokra** vonatkozó házirend: az Amerikai Egyesült államokbeli útlevél száma 123456789

Ha szeretne többet megtudni arról, hogy mire van szükség egy amerikai/brit Passport-számhoz a tartalomhoz, olvassa el a következő cikket: [Mi a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Ha más beépített bizalmas adattípust használ, további információt a következő témakörben talál: [a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  