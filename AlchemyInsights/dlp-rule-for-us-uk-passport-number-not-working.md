---
title: DLP szabály az USA/Uk útlevélszám nem működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931264"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problémák a DLP - USA / Uk útlevél számok

**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben. Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások. Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.

Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon. Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben. Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.

**DLP kérdések az USA/Egyesült Királyság útlevélszámokkal**

Problémái vannak az **adatveszteség-megelőzéssel (DLP),** amely nem működik **az egyesült államokbeli/egyesült királyságbeli útlevélszámot** tartalmazó tartalom esetében, amikor Az O365-ben DLP-érzékeny információtípust használ? Ha igen, győződjön meg arról, hogy a tartalom tartalmazza a szükséges információkat, amit a DLP-házirend keres, amikor kiértékeli.
  
Például egy 75%-os megbízhatósági szinttel konfigurált **egyesült államokbeli/brit útlevélszám-házirend** esetében a rendszer kiértékeli a következőket, és a szabály aktiválásához észlelni kell őket.
  
- **[Formátum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Kilenc számjegy

- **[Minta:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Kilenc egymást követő számjegy

- **[Ellenőrző összeg:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nem, nincs Checksum

- **[Meghatározás:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP-házirend 75%-ban biztos abban, hogy az ilyen típusú bizalmas információkat észleli, ha 300 karakteren belül:

  - A Func_usa_uk_passport függvény a mintának megfelelő tartalmat talál.

  - A Keyword_passport kulcsszó található.

    Például a következő minta váltaná ki az **Egyesült Államok/Egyesült Királyság útlevélszámra** vonatkozó politikáját: U.S. Passport number 123456789

Ha többet szeretne tudni arról, hogy mi szükséges az Egyesült Államok/Egyesült Királyság útlevélszám észleléséhez a tartalomhoz, olvassa el a cikk következő szakaszát: [A bizalmas információtípusok az USA/UK útlevélszámát keresik?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Egy másik beépített bizalmas információtípus használatával a következő cikkben további információt talál arról, hogy mi szükséges más típusokhoz: [Mit keresnek a bizalmas információtípusok?](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  