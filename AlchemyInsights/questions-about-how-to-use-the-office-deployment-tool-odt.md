---
title: Az Office Deployment Tool (ODT) használatával kapcsolatos kérdések
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553542"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Az Office Deployment Tool (ODT) használatával kapcsolatos kérdések

Az Office Deployment eszköz letölthető a [Microsoft letöltőközpontból](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
A fájl letöltése után futtassa az önkicsomagoló végrehajtható fájl, amely tartalmazza az Office telepítési eszköz futtatható (setup.exe) és egy minta konfigurációs fájl (configuration.xml).
  
 **Zárja ki, vagy távolítsa el az Office 365 ProPlus termékek az ügyfélszámítógépek:**
  
Ha telepíti az Office 365 ProPlus, meghatározott termékekre is kizárhat. Ehhez kövesse az ODT az Office telepítésének, de a ExcludeApp elem tartalmazza a konfigurációs fájlban. Ez a konfigurációs fájl például az Office 365 ProPlus termékek, kivéve a Publisher telepíti:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Az Office Deployment eszköz – áttekintés](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

