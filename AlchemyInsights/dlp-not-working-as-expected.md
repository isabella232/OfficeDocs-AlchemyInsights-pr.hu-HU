---
title: A DLP nem a várt módon működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704415"
---
# <a name="dlp-not-working-as-expected"></a>A DLP nem a várt módon működik

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

 **A DLP beállítása**

Problémái vannak az **adatvesztés-megelőzéssel (DLP)** az Office 365-ben, hogy nem a várt módon működnek? Ha igen, győződjön meg arról, hogy a **DLP-házirend** megfelelően van beállítva, és hogy az adatok tartalmazzák, amit a **DLP-házirend** keres, amikor kiértékelik.
  
A DLP-házirendek lehetővé teszik a szervezeten belüli bizalmas adatok azonosítását és védelmét. A DLP-házirendek beállításához használja az [itt](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)található információkat.
  
 **Mit keresnek a DLP-házirendek?**
  
A biztonsági és megfelelőségi központok **beépített bizalmas információtípusainak** használatakor a DLP-házirendek az ilyen bizalmas típusok észlelésekor konkrét mintákat és elemeket keresnek.
  
- **Beépített bizalmas információtípusok**

    A beépített bizalmas típusokról és a DLP-házirend ről a Bizalmas típus észlelésekor a következő témakörben talál tájékoztatást: [A bizalmas információtípusok keresetttémaköre.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)

- **Egyéni bizalmas információtípusok**

    Ha egyéni bizalmas információtípusokat próbál létrehozni, az alábbi cikkben megtudhatja, hogyan hozhat létre egyéni bizalmas [szöveget: Egyéni bizalmas információtípus létrehozása](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**DLP-házirend tesztelése**

Ha az adatokat beépített vagy egyéni bizalmas adatoktípussal szeretné tesztelni, használja a **Teszttípus** beállítást a **Besorolások** > **bizalmas információtípusai**csoportban. További információt az [Egyéni bizalmas információtípusok tesztelése](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)című témakörben talál.

 **Jelentések**
  
- Bizalmas adatok betekintést nyerhet a [DLP-jelentések segítségével.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Az esemény konkrét részleteinek megtekintése [incidensjelentéssel.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)
