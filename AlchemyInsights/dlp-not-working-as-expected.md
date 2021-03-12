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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707812"
---
# <a name="dlp-not-working-as-expected"></a>A DLP nem a várt módon működik

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

 **A DLP beállítása**

Az Office 365 **adatveszteség-megelőzési (DLP)** problémái nem a várt módon működnek? Ha igen, győződjön meg arról, hogy a **DLP-házirend** megfelelően van beállítva, és hogy az adatok azt tartalmazják, amit a **DLP-házirend** a kiértékeléskor keres.
  
A DLP-házirendek lehetővé teszik a bizalmas adatok azonosítását és védelmét a szervezetben. A DLP-házirendek beállításához használja az itt [található információkat.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Milyen DLP-házirendeket keresnek?**
  
Amikor a biztonsági és megfelelőségi központok beépített bizalmas adattípusokat használ, a **DLP-házirendek** meghatározott mintákat és elemeket keresnek a bizalmas típusok észlelése során.
  
- **Beépített bizalmas információtípusok**

    A bizalmas típusú adatok beépített típusairól és arról, hogy a DLP-házirend mit keres a Bizalmas típus észlelése esetén: A bizalmas [adattípusok által kereshető információk.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Egyéni bizalmas információtípusok**

    Ha egyéni bizalmas adattípusokat próbál létrehozni, az alábbi cikkben további információt talál az egyéni bizalmas adattípusok létrehozásáról: Egyéni bizalmas adattípus [létrehozása.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**DLP-házirend tesztelése**

Ha egy beépített vagy egyéni bizalmasadat-típussal tesztelni kívánt adatokat, használja a Bizalmas adatok besorolása csoport Teszttípus   >  **beállítását.** További információt az egyéni bizalmas [adattípusok tesztelése.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Jelentések**
  
- Bizalmas adatelemzéseket kaphat a [DLP-jelentésekkel.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Az esemény részleteinek megtekintése [incidensjelentéssel.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
