---
title: Az Office-telepítő eszköz használata
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
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085834"
---
# <a name="using-the-office-deployment-tool-odt"></a>Az Office-telepítő eszköz használata (ODT)

Az Office-telepítő eszköz (ODT) segítségével telepítheti az Office 365 Office-verzióit. Az Office-telepítő eszköz (setupodt.exe) a parancssorból futtatható, és egy konfigurációs XML-fájlt használ annak meghatározásához, hogy milyen beállítások vonatkoznak az Office telepítésekor.
  
1. Töltse le az Office-telepítő eszköz legújabb verzióját a [Microsoft letöltőközpontból](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Az [Office customization Tool (TOT)](https://config.office.com) segítségével jelölje ki a központi telepítő beállításait, és hozza létre a konfigurációs XML-fájlt. Exportálja a konfigurációs fájlt, és helyezze azt helyileg ugyanarra a mappába, ahol a setupodt.exe található.

    **Megjegyzés:** Az Office telepítési problémái gyakran előfordulnak a helytelenül konfigurált vagy malformatted konfigurációs fájlok miatt. Az ilyen problémák elkerülése érdekében az Office customization Tool segítségével hozza létre a konfigurációs fájlt. A meglévő konfigurációs fájlokat is importálhatja az Office customization Tool alkalmazásba.

3. Egy rendszergazdai jogú parancssorból váltson arra a helyre, ahol a setupodt.exe-ban lakik, és futtassa az Office-telepítő eszközt a letöltési módban, és adja meg az imént mentett konfigurációs fájlt. Ebben a példában a konfigurációs fájl neve Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. Futtassa az Office-telepítő eszközt a konfigurálás módban, és adja meg a konfigurációs fájlt.

```setupodt.exe /configure Configuration.xml```

**Megjegyzés:** Ezt a lépést az ügyfélgépről kell futtatnia, amelyen telepíteni szeretné az Office-t, és a számítógépen helyi rendszergazdai engedélyekkel kell rendelkeznie.

Ha többet szeretne tudni az Office-telepítő eszköz használatáról a Microsoft 365-alkalmazásaiban a nagyvállalati telepítéshez, olvassa el [az Office-telepítő eszköz áttekintése](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)című témakört. Az Office customization Tool használatáról további információt [az Office customization Tool áttekintése](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)című témakörben talál.
