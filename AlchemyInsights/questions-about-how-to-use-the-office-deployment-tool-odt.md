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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="a33c0-102">Az Office deployment tool (ODT) használatával kapcsolatos kérdések</span><span class="sxs-lookup"><span data-stu-id="a33c0-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="a33c0-103">Töltse le az Office telepítőeszközt a [Microsoft letöltőközpontjából.](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="a33c0-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="a33c0-104">A fájl letöltése után futtassa az önkicsomagoló végrehajtható fájlt, amely tartalmazza az Office deployment tool végrehajtható fájlját (setup.exe) és egy konfigurációs mintafájlt (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="a33c0-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="a33c0-105">**A Microsoft 365 nagyvállalati alkalmazások kizárása vagy eltávolítása az ügyfélszámítógépekről:**</span><span class="sxs-lookup"><span data-stu-id="a33c0-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="a33c0-106">A Microsoft 365 nagyvállalati alkalmazások telepítésekor kizárhat bizonyos termékeket.</span><span class="sxs-lookup"><span data-stu-id="a33c0-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="a33c0-107">Ehhez kövesse az Office ODT-val történő telepítésének lépéseit, de foglalja bele az ExcludeApp elemet a konfigurációs fájlba.</span><span class="sxs-lookup"><span data-stu-id="a33c0-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="a33c0-108">Ez a konfigurációs fájl például a Publisher kivételével telepíti az összes Microsoft 365-ös alkalmazást a vállalati termékekhez:</span><span class="sxs-lookup"><span data-stu-id="a33c0-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="a33c0-109">Az Office telepítőeszközének áttekintése</span><span class="sxs-lookup"><span data-stu-id="a33c0-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

