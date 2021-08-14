---
title: A vállalati telepítőeszköz (ODT) Office használata
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959685"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>A vállalati telepítőeszköz (ODT) Office használata

Töltse le Office telepítőeszközt a [Microsoft letöltőközpontból.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
A fájl letöltése után futtassa az önkigyűjő végrehajtható fájlt, amely tartalmazza az Office-telepítő eszköz végrehajtható fájlját (setup.exe) és egy konfigurációs mintafájlt (configuration.xml).
  
 **A termékek ügyfélszámítógépről Nagyvállalati Microsoft 365-alkalmazások kizárása vagy eltávolítása:**
  
A Nagyvállalati Microsoft 365-alkalmazások kizárhat bizonyos termékeket. Kövesse az ODT-fájllal való Office, de a konfigurációs fájlba foglalja bele az ExcludeApp elemet. Ez a konfigurációs fájl például az összes Nagyvállalati Microsoft 365-alkalmazások, kivéve a Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[A Office áttekintése](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

