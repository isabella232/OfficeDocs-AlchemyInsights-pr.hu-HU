---
title: A DLP nem a várt módon működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932624"
---
# <a name="dlp-not-working-as-expected"></a>A DLP nem a várt módon működik

**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben. Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások. Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.

Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon. Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben. Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.

 **A DLP beállítása**

Problémái vannak az **adatvesztés-megelőzéssel (DLP)** az Office 365-ben, hogy nem a várt módon működnek? Ha igen, győződjön meg arról, hogy a **DLP-házirend** megfelelően van beállítva, és hogy az adatok tartalmazzák, amit a **DLP-házirend** keres, amikor kiértékelik.
  
A DLP-házirendek lehetővé teszik a szervezeten belüli bizalmas adatok azonosítását és védelmét. A DLP-házirendek beállításához használja az [itt](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)található információkat.
  
 **Mit keresnek a DLP-házirendek?**
  
Ha az Office 365 Biztonsági és megfelelőségi központban **a beépített bizalmas információtípusokat** használja, a DLP-házirendek az ilyen bizalmas típusok észlelésekor konkrét mintákat és elemeket keresnek.
  
- **Beépített bizalmas információtípusok**

    A beépített bizalmas típusokról és a DLP-házirend ről a Bizalmas típus észlelésekor a következő témakörben talál tájékoztatást: [A bizalmas információtípusok keresetttémaköre.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)

- **Egyéni bizalmas információtípusok**

    Ha egyéni bizalmas információtípusokat próbál létrehozni, az alábbi cikkben megtudhatja, hogyan hozhat létre egyéni bizalmas [szöveget: Egyéni bizalmas információtípus létrehozása](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**DLP-házirend tesztelése**

Ha az adatokat beépített vagy egyéni bizalmas adatoktípussal szeretné tesztelni, használja a **Teszttípus** beállítást a **Besorolások** > **bizalmas információtípusai**csoportban. További információt az [Egyéni bizalmas információtípusok tesztelése](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)című témakörben talál.

 **Jelentések**
  
- Bizalmas adatok betekintést nyerhet a [DLP-jelentések segítségével.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Az esemény konkrét részleteinek megtekintése [incidensjelentéssel.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)
