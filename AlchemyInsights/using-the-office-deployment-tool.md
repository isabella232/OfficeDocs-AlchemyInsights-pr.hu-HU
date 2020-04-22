---
title: Az Office-telepítő eszköz használata
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726250"
---
# <a name="using-the-office-deployment-tool-odt"></a>Az Office-telepítő eszköz (ODT) használata

Az Office-telepítő eszközzel (ODT) telepítheti az Office 365 Office-verzióit. Az Office deployment tool (setup.exe) parancssorból fut, és egy konfigurációs XML-fájl segítségével határozza meg, hogy milyen beállításokat kell alkalmazni az Office telepítésekor.
  
1. Töltse le az Office telepítőeszköz legújabb verzióját a [Microsoft letöltőközpontjából.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Az [Office testreszabási eszközével (OCT)](https://config.office.com) kiválaszthatja a telepítési beállításokat, és létrehozhatja a konfigurációs XML-fájlt. Exportálja a konfigurációs fájlt, és helyezze helyileg ugyanarra a mappára, ahol a setup.exe található.

    **Megjegyzés:** Az Office telepítésével kapcsolatos problémák gyakran a helytelenül konfigurált vagy helytelenül formázott konfigurációs fájlok miatt jelentkeznek. Az ilyen problémák elkerülése érdekében javasoljuk, hogy az Office testreszabási eszközével hozza létre a konfigurációs fájlt. Meglévő konfigurációs fájlokat is importálhat az Office testreszabási eszközébe.

3. A rendszergazda jogú parancssorból váltson arra a helyre, ahol a setup.exe található, és futtassa az Office-telepítési eszközt letöltési módban, és adja meg az imént mentett konfigurációs fájlt. Ebben a példában a konfigurációs fájl neve Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Futtassa az Office-telepítő eszközt konfigurálási módban, és adja meg a konfigurációs fájlt.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Megjegyzés:** Ezt a lépést arról az ügyfélszámítógépről kell futtatnia, amelyre telepíteni szeretné az Office-t, és helyi rendszergazdai engedélyekkel kell rendelkeznie a számítógépen.

Ha többet szeretne tudni arról, hogy miként használható az Office-telepítő eszköz a Microsoft 365-alkalmazásokhoz vállalati telepítési helyzetekben, olvassa [el az Office-telepítési eszköz áttekintése című témakört.](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool) Az Office testreszabási eszközének használatáról az [Office testreszabási eszköz áttekintése című témakörben olvashat bővebben.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
