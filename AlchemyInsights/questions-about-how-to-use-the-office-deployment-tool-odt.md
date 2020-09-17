---
title: Az Office-telepítő eszköz (ODT) használatának kérdései
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774893"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Az Office-telepítő eszköz (ODT) használatának kérdései

Töltse le az Office-telepítő eszközt a [Microsoft letöltőközpontból](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Miután letöltötte a fájlt, futtassa az önkicsomagoló végrehajtható fájlt, amely tartalmazza az Office-telepítő eszköz végrehajtható fájlját (setup.exe) és egy minta konfigurációs fájlt (configuration.xml).
  
 **A Microsoft 365-alkalmazások kihagyása vagy eltávolítása a nagyvállalati termékekből az ügyfélgépekről:**
  
A Microsoft 365-alkalmazások nagyvállalatoknak való telepítésekor kihagyhatja az adott termékeket. Ehhez kövesse az Office-nak az ODT szolgáltatással való telepítéséhez szükséges lépéseket, de vegye fel a ExcludeApp elemet a konfigurációs fájlban. Ez a konfigurációs fájl például a Publisher kivételével a Microsoft 365-alkalmazásokat telepíti a nagyvállalati termékekhez:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Az Office-telepítő eszköz áttekintése](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

