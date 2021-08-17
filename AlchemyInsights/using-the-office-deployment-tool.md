---
title: A Office eszköz használata
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083772"
---
# <a name="using-the-office-deployment-tool-odt"></a>A Office (ODT) használata

A Office (ODT) segítségével telepítheti Office 365 verziókat a Office. A Office telepítőeszköz (setup.exe) parancssorból fut, és egy konfigurációs XML-fájl segítségével határozza meg, hogy milyen beállításokat kell alkalmazni a Office.
  
1. Töltse le a Office telepítőeszköz legújabb verzióját a [Microsoft letöltőközpontból.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. A Office [(OCT)](https://config.office.com) használatával adja meg a telepítési beállításokat, és hozza létre a konfigurációs XML-fájlt. Exportálja a konfigurációs fájlt, és helyezze helyileg arra a mappára, amelyben a setup.exe található.

    **Megjegyzés:** Office telepítési hibákat gyakran az rosszul konfigurált vagy hibásan formázott konfigurációs fájlok okozhatják. Az ilyen problémák elkerülése érdekében azt javasoljuk, hogy a Office testreszabási eszközzel hozza létre a konfigurációs fájlt. Meglévő konfigurációs fájlokat is importálhat a Office eszközbe.

3. Az emelt szintű parancssorból váltson arra a helyre, Office setup.exe a telepítőeszközt letöltési módban futtassa, és adja meg a mentett konfigurációs fájlt. Ebben a példában a konfigurációs fájl neve Configuration.xml:

```setup.exe /download Configuration.xml```

4.Futtassa a Office telepítőeszközt konfigurálási módban, és adja meg a konfigurációs fájlt.

```setup.exe /configure Configuration.xml```

**Megjegyzés:** Ezt a lépést az ügyfélszámítógépről kell futtatnia, amelyen telepíteni szeretné Office és helyi rendszergazdai engedélyekkel kell rendelkeznie az adott számítógépen.

Ha többet szeretne megtudni a Office eszköz Nagyvállalati Microsoft 365-alkalmazások telepítési esetekhez, olvassa el A központi telepítőeszköz Office [áttekintése témakört.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) A testre szabható eszköz Office az Overview [of the Office (Egyéni](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)testreszabási eszköz) Office olvashat.
