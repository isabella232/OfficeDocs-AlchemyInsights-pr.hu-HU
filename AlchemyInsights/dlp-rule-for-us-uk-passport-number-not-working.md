---
title: DLP szabály az USA/Uk útlevélszám nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507300"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problémák a DLP - USA / Uk útlevél számok

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**DLP kérdések az USA/Egyesült Királyság útlevélszámokkal**

Problémái vannak az **adatveszteség-megelőzéssel (DLP),** amely nem működik **az egyesült államokbeli/egyesült királyságbeli útlevélszámot** tartalmazó tartalom esetében, amikor Az O365-ben DLP-érzékeny információtípust használ? Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a szükséges információkat, amit a DLP-házirend keres, amikor kiértékeli.
  
Például egy 75%-os megbízhatósági szinttel konfigurált **egyesült államokbeli/brit útlevélszám-házirend** esetében a rendszer kiértékeli a következőket, és a szabály aktiválásához észlelni kell őket.
  
- **[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Kilenc számjegy

- **[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Kilenc egymást követő számjegy

- **[Ellenőrző összeg:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nem, nincs Checksum

- **[Meghatározás:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP-házirend 75%-ban biztos abban, hogy az ilyen típusú bizalmas információkat észleli, ha 300 karakteren belül:

  - A Func_usa_uk_passport függvény a mintának megfelelő tartalmat talál.

  - A Keyword_passport kulcsszó található.

    Például a következő minta váltaná ki az **Egyesült Államok/Egyesült Királyság útlevélszámra** vonatkozó politikáját: U.S. Passport number 123456789

Ha többet szeretne tudni arról, hogy mi szükséges az Egyesült Államok/Egyesült Királyság útlevélszám észleléséhez a tartalomhoz, olvassa el a cikk következő szakaszát: [A bizalmas információtípusok az USA/UK útlevélszámát keresik?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Egy másik beépített bizalmas információtípus használatával a következő cikkben további információt talál arról, hogy mi szükséges más típusokhoz: [Mit keresnek a bizalmas információtípusok?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  