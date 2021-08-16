---
title: Nem működő egyesült királyságbeli útlevélszámra vonatkozó DLP-szabály
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004948"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problémák a DLP - EGYESÜLT királyságbeli útlevélszámokkal

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**Egyesült királyságbeli útlevélszámokkal kapcsolatos DLP-problémák**

Nem működik az adatveszteség-megelőzési **(DLP)** probléma  az Egyesült Királyságban érvényes egyesült királyságbeli útlevélszámmal rendelkező tartalommal kapcsolatban, ha bizalmas adattípust használ az O365-ben? Ebben az esetben győződjön meg arról, hogy a tartalom tartalmazza azokat az információkat, amelyekre a DLP-házirend értékelésekor szüksége van.
  
Egy 75%-os megbízhatósági szinttel konfigurált EGYESÜLT KIRÁLYSÁG-beli útlevélszám-házirend esetén például az alábbiakat értékeli ki a rendszer, és a szabály csak akkor aktiválódik, ha a szabály aktiválódik: 
  
- **[Formátum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Kilenc számjegy

- **[Minta:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Kilenc egymást követő számjegy

- **[Ellenőrzőum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nem, nincs Ellenőrzőum

- **[Definíció:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP-házirend 75%-os magabiztosan észleli ezt a típusú bizalmas információt, ha 300 karakteren belül:

  - A függvény Func_usa_uk_passport mintára illeszkedő tartalmat talál.

  - Található egy Keyword_passport.

    Az Egyesült Államok/Egyesült Királyság  útlevélszámára vonatkozó szabályzat esetében például a következő minta lép fel: Amerikai Útlevélszám 123456789

Ha további információra van szüksége arról, hogy mi szükséges ahhoz, hogy a rendszer [](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) észlelni tudja az Egyesült Királyságbeli útlevélszámokat a tartalomhoz, tekintse meg a jelen cikk következő szakaszát: Az egyesült királyságbeli útlevélszámok bizalmas adattípusa
  
Más, beépített bizalmas információtípust használva a következő cikkben talál információt a más típusokhoz szükséges információkról: Mit keresnek a bizalmas [adattípusok?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  