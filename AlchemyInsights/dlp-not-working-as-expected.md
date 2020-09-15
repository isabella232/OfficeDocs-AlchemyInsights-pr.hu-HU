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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679695"
---
# <a name="dlp-not-working-as-expected"></a>A DLP nem a várt módon működik

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

 **DLP beállítása**

Problémát tapasztal az **adatvesztés-megelőzés (DLP)** használatakor az Office 365-ben, nem a várt módon működik? Ha igen, győződjön meg arról, hogy a **DLP-házirend** megfelelően van beállítva, és hogy az Ön által kiértékeléskor az Ön által használt **DLP-házirend** milyen információkat tartalmaz.
  
A DLP-házirendekkel bizalmas információkat azonosíthat és védheti meg a szervezetében. A DLP-házirendek beállításához használja az [alábbi](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)információkat.
  
 **Milyen DLP-házirendeket keres**
  
A biztonsági és megfelelőségi központokban a **beépített bizalmas adattípusok** használatakor a DLP-házirendek bizonyos mintázatokat és elemeket keresnek a bizalmas típusok észlelése során.
  
- **Beépített bizalmas adattípusok**

    A beépített bizalmas típusokról, valamint arról, hogy milyen típusú DLP-házirendet keres a bizalmas típus észlelése során, a következő témakörben talál információt: [a bizalmas adattípusok keresése](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Egyéni bizalmas adattípusok**

    Ha egyéni bizalmas adattípusokat próbál létrehozni, az alábbi cikkből megtudhatja, hogy miként hozhat létre egyéni bizalmas típust: [Egyéni bizalmas adattípus létrehozása](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**DLP-házirend tesztelése**

Ha egy beépített vagy egyéni bizalmas adattípussal szeretné tesztelni az adatokat, használja a **típus típusa** beállítást a bizalmas adatok **osztályozása**csoportban  >  **Sensitive info types**. További információt az [Egyéni bizalmas adattípusok tesztelése](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)című témakörben találhat.

 **Jelentések**
  
- Az adatok bizalmasan jelennek meg [DLP-jelentésekkel.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Az esemény konkrét részleteinek megtekintése incidens- [jelentéssel](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
