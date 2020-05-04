---
title: Az Office deployment tool (ODT) használatával kapcsolatos kérdések
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010751"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Az Office deployment tool (ODT) használatával kapcsolatos kérdések

Töltse le az Office telepítőeszközt a [Microsoft letöltőközpontjából.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
A fájl letöltése után futtassa az önkicsomagoló végrehajtható fájlt, amely tartalmazza az Office deployment tool végrehajtható fájlját (setup.exe) és egy konfigurációs mintafájlt (configuration.xml).
  
 **A Microsoft 365 nagyvállalati alkalmazások kizárása vagy eltávolítása az ügyfélszámítógépekről:**
  
A Microsoft 365 nagyvállalati alkalmazások telepítésekor kizárhat bizonyos termékeket. Ehhez kövesse az Office ODT-val történő telepítésének lépéseit, de foglalja bele az ExcludeApp elemet a konfigurációs fájlba. Ez a konfigurációs fájl például a Publisher kivételével telepíti az összes Microsoft 365-ös alkalmazást a vállalati termékekhez:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Az Office telepítőeszközének áttekintése](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

