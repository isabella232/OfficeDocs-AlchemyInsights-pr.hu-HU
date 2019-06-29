---
title: Az Office Deployment eszközzel
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365527"
---
# <a name="using-the-office-deployment-tool-odt"></a>Az Office Deployment Tool (ODT eszköz) használatával

Az Office Deployment Tool (ODT) segítségével Office Office 365 változatának telepítését. Az Office telepítési eszköz (setup.exe) futtatása a parancssorból, és egy konfigurációs XML-fájlt használja annak megállapítására, milyen beállításokat alkalmazza az Office telepítésekor.
  
1. Töltse le az Office telepítési eszköz legújabb verzióját a [Microsoft Download Center webhelyről](http://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Az [Office testreszabási eszközének (TOT)](https://config.office.com) segítségével lehet megadni a telepítési beállításokat és a konfigurációs XML-fájl létrehozása. Exportálja a konfigurációs fájlt, és helyileg tegyük ugyanabba a mappába, ahol a setup.exe található.

    **Megjegyzés:** Office telepítési problémák gyakran következnek be, hogy rosszul van konfigurálva vagy malformatted konfigurációs fájlokat. Az ilyen problémák elkerülése érdekében azt javasoljuk, hogy az Office testreszabási eszközének segítségével hozza létre a konfigurációs fájlt. Meglévő konfigurációs fájlok is importálhatók az Office testreszabási eszközének.

3. Egy emelt szintű parancssorból váltson arra a helyre, ahol az található setup.exe és az Office telepítési eszköz letöltési módban fut, és adja meg a mentett konfigurációs fájl. Ebben a példában a konfigurációs fájl neve Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Az Office Deployment eszköz mód beállítása, és adja meg a konfigurációs fájlban.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Megjegyzés:** Ebben a lépésben az ügyfélszámítógépről szeretné telepíteni az Office és helyi rendszergazdai jogosultságokkal kell rendelkeznie a számítógépen kell futtatni.

Az Office 365 ProPlus elképzelések Office telepítési eszköz használatával kapcsolatban további tudnivalókat [az Office telepítési eszköz – áttekintés](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)című témakörben talál. Az Office testreszabási eszközének használatáról további tudnivalókat talál [az Office testreszabási eszközének áttekintése](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
