---
title: Az Office Deployment Tool (ODT) eszköz használatára vonatkozó kérdések
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553542"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Az Office Deployment Tool (ODT) eszköz használatára vonatkozó kérdések

Töltse le az Office telepítőeszközét a [Microsoft letöltőközpontjából](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
A fájl letöltése után futtassa az önkicsomagoló végrehajtható fájlt, amely tartalmazza az Office telepítő végrehajtható fájlját (Setup. exe) és egy konfigurációs mintafájlt (Configuration. xml).
  
 **-Hoz kizár vagy eltávolít Hivatal 365 ProPlus termékek-ból ügyfél számítógépek:**
  
Mikor beiktatás Hivatal 365 ProPlus, tudod kizár különleges termékek. Ehhez kövesse az Office és az ODT telepítésének lépéseit, de adja meg az ExcludeApp elemet a konfigurációs fájlban. Például, ez a konfigurációs fájl telepíti az összes Office 365 ProPlus termékek, kivéve a Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Az Office-telepítőeszköz áttekintése](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

