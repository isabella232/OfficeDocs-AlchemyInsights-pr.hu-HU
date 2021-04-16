---
title: Az Office-telepítő eszköz (ODT) használatával kapcsolatos kérdések
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790334"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Az Office-telepítő eszköz (ODT) használatával kapcsolatos kérdések

Töltse le az Office-telepítő eszközt a [Microsoft letöltőközpontból.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
A fájl letöltése után futtassa az önkigyűjő végrehajtható fájlt, amely tartalmazza az Office-telepítő eszköz végrehajtható fájlját (setup.exe) és egy konfigurációs mintafájlt (configuration.xml).
  
 **A nagyvállalati termékekhez használt Microsoft 365-alkalmazások ügyfélszámítógépeken való kizárása vagy eltávolítása:**
  
A Nagyvállalati Microsoft 365-alkalmazások telepítésekor kizárhat bizonyos termékeket. Kövesse az Office ODT-fájllal való telepítésének lépéseit, de a konfigurációs fájlba foglalja bele az ExcludeApp elemet. Ez a konfigurációs fájl például telepíti az összes Nagyvállalati Microsoft 365-appot, kivéve a Publishert:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Az Office-telepítő eszköz áttekintése](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

