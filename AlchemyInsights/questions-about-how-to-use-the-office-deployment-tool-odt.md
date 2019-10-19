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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="e4012-102">Az Office Deployment Tool (ODT) eszköz használatára vonatkozó kérdések</span><span class="sxs-lookup"><span data-stu-id="e4012-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="e4012-103">Töltse le az Office telepítőeszközét a [Microsoft letöltőközpontjából](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="e4012-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="e4012-104">A fájl letöltése után futtassa az önkicsomagoló végrehajtható fájlt, amely tartalmazza az Office telepítő végrehajtható fájlját (Setup. exe) és egy konfigurációs mintafájlt (Configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="e4012-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="e4012-105">**-Hoz kizár vagy eltávolít Hivatal 365 ProPlus termékek-ból ügyfél számítógépek:**</span><span class="sxs-lookup"><span data-stu-id="e4012-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="e4012-106">Mikor beiktatás Hivatal 365 ProPlus, tudod kizár különleges termékek.</span><span class="sxs-lookup"><span data-stu-id="e4012-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="e4012-107">Ehhez kövesse az Office és az ODT telepítésének lépéseit, de adja meg az ExcludeApp elemet a konfigurációs fájlban.</span><span class="sxs-lookup"><span data-stu-id="e4012-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="e4012-108">Például, ez a konfigurációs fájl telepíti az összes Office 365 ProPlus termékek, kivéve a Publisher:</span><span class="sxs-lookup"><span data-stu-id="e4012-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="e4012-109">Az Office-telepítőeszköz áttekintése</span><span class="sxs-lookup"><span data-stu-id="e4012-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

