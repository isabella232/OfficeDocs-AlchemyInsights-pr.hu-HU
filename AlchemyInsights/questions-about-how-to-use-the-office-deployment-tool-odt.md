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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="f9b86-102">Az Office-telepítő eszköz (ODT) használatának kérdései</span><span class="sxs-lookup"><span data-stu-id="f9b86-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="f9b86-103">Töltse le az Office-telepítő eszközt a [Microsoft letöltőközpontból](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="f9b86-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="f9b86-104">Miután letöltötte a fájlt, futtassa az önkicsomagoló végrehajtható fájlt, amely tartalmazza az Office-telepítő eszköz végrehajtható fájlját (setup.exe) és egy minta konfigurációs fájlt (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="f9b86-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="f9b86-105">**A Microsoft 365-alkalmazások kihagyása vagy eltávolítása a nagyvállalati termékekből az ügyfélgépekről:**</span><span class="sxs-lookup"><span data-stu-id="f9b86-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="f9b86-106">A Microsoft 365-alkalmazások nagyvállalatoknak való telepítésekor kihagyhatja az adott termékeket.</span><span class="sxs-lookup"><span data-stu-id="f9b86-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="f9b86-107">Ehhez kövesse az Office-nak az ODT szolgáltatással való telepítéséhez szükséges lépéseket, de vegye fel a ExcludeApp elemet a konfigurációs fájlban.</span><span class="sxs-lookup"><span data-stu-id="f9b86-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="f9b86-108">Ez a konfigurációs fájl például a Publisher kivételével a Microsoft 365-alkalmazásokat telepíti a nagyvállalati termékekhez:</span><span class="sxs-lookup"><span data-stu-id="f9b86-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="f9b86-109">Az Office-telepítő eszköz áttekintése</span><span class="sxs-lookup"><span data-stu-id="f9b86-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

