---
title: A DLP nem a várt módon működik
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079704"
---
# <a name="dlp-not-working-as-expected"></a>A DLP nem a várt módon működik

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

 **A DLP beállítása**

Az adatveszteség-megelőzéssel **(DLP)** kapcsolatos problémákat tapasztal a Office 365 nem a várt módon működik? Ha igen, ellenőrizze, hogy a **DLP-házirend** megfelelően van-e beállítva, és hogy az adatok azt tartalmaznak, amit a **DLP-házirend** keres a kiértékeléskor.
  
A DLP-házirendekkel azonosíthatja és megvédheti a bizalmas adatokat a szervezetében. DLP-házirendek beállításához használja az itt [található információkat.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **A DLP-házirendek által keresve**
  
Ha a biztonsági és megfelelőségi központok beépített bizalmas adattípusokat használ, a **DLP-házirendek** meghatározott mintákat és elemeket keresnek a bizalmas típusú adatok észlelésekor.
  
- **Beépített bizalmas adattípusok**

    A beépített Bizalmas típusú adatokról és arról, hogy a DLP-házirend mit keres a Bizalmas típus észlelése esetén, a következőt lásd: A bizalmas [adattípusok által kereshető információk.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Egyéni bizalmas adattípusok**

    Ha egyéni bizalmas adattípusokat próbál létrehozni, a következő cikkben talál további információt az egyéni bizalmas adattípusok létrehozásáról: Egyéni bizalmas adattípus [létrehozása.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**DLP-házirend tesztelése**

Ha egy beépített vagy egyéni bizalmasadat-típussal tesztelni kívánt adatokat, használja a Teszttípus lehetőséget a **Besorolások** bizalmas adatok típusai   >  **csoportban.** További információ: Egyéni bizalmas [adattípusok tesztelése.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Jelentések**
  
- A DLP-jelentésekkel bizalmas [adatelemzéseket kaphat.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Az esemény részleteinek megtekintése az [Incidensjelentéssel.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
