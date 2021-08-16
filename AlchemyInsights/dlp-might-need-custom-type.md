---
title: Előfordulhat, hogy a DLP-nek egyéni típusra van szüksége
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030796"
---
# <a name="dlp-might-need-a-custom-type"></a>Előfordulhat, hogy a DLP-nek egyéni típusra van szüksége

**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.

**A DLP egyéni adattípust is megkövetelhet**

Az adatveszteség-megelőzési (DLP)-házirendekkel azonosíthatja és megvédheti a bizalmas adatokat a szervezetében. Bizonyos esetekben előfordulhat, hogy létre kell  hoznia egy saját bizalmasadat-típust a szervezet adatainak védelméhez.

Előfordulhat például, hogy a szervezetnek azonosítania és védenie kell az alkalmazotti azonosítókat vagy más adatokat a szervezetére jellemző bizonyos formátumban. Ha igen, további információt az alábbi cikkekben talál.
  
 **Beépített bizalmas adattípus testreszabása**
  
Ha egy beépített bizalmas adattípus csupán néhány finomítással kielégíti az igényeit, testre szabhatja a beépített bizalmas [adattípusokat.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Felvehet vagy eltávolíthat például kulcsszavakat, illetve hozzáadhat vagy eltávolíthat támogató bizonyítékokat, például dátumot vagy címet.
  
 **Egyéni bizalmas adattípus létrehozása**
  
Ha azonban egy másik bizalmas információtípust kell azonosítania és védenie, létrehozhat egy egyéni bizalmas információtípust [a](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) Biztonsági és megfelelőségi központ & felhasználói felületén.
  
**Egyéni bizalmas információtípus létrehozása a Biztonsági & PowerShellben**

Végül, ha a felhasználói felület nem biztosít minden szükséges lehetőséget, létrehozhat egy egyéni bizalmas adattípust [a Biztonsági & PowerShellben.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) Xml-fájllal kezdődően minden elérhető beállítást használhat.
