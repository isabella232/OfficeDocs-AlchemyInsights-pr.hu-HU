---
title: Az Office Deployment eszközzel
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423185"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="ae362-102">Az Office Deployment Tool (ODT eszköz) használatával</span><span class="sxs-lookup"><span data-stu-id="ae362-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="ae362-103">Az Office Deployment Tool (ODT) segítségével Office Office 365 változatának telepítését.</span><span class="sxs-lookup"><span data-stu-id="ae362-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="ae362-104">Az Office telepítési eszköz (setup.exe) futtatása a parancssorból, és egy konfigurációs XML-fájlt használja annak megállapítására, milyen beállításokat alkalmazza az Office telepítésekor.</span><span class="sxs-lookup"><span data-stu-id="ae362-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="ae362-105">Töltse le az Office telepítési eszköz legújabb verzióját a [Microsoft Download Center webhelyről](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="ae362-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="ae362-106">Az [Office testreszabási eszközének (TOT)](https://config.office.com) segítségével lehet megadni a telepítési beállításokat és a konfigurációs XML-fájl létrehozása.</span><span class="sxs-lookup"><span data-stu-id="ae362-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="ae362-107">Exportálja a konfigurációs fájlt, és helyileg tegyük ugyanabba a mappába, ahol a setup.exe található.</span><span class="sxs-lookup"><span data-stu-id="ae362-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="ae362-108">**Megjegyzés:** Office telepítési problémák gyakran következnek be, hogy rosszul van konfigurálva vagy malformatted konfigurációs fájlokat.</span><span class="sxs-lookup"><span data-stu-id="ae362-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="ae362-109">Az ilyen problémák elkerülése érdekében azt javasoljuk, hogy az Office testreszabási eszközének segítségével hozza létre a konfigurációs fájlt.</span><span class="sxs-lookup"><span data-stu-id="ae362-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="ae362-110">Meglévő konfigurációs fájlok is importálhatók az Office testreszabási eszközének.</span><span class="sxs-lookup"><span data-stu-id="ae362-110">You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="ae362-111">Egy emelt szintű parancssorból váltson arra a helyre, ahol az található setup.exe és az Office telepítési eszköz letöltési módban fut, és adja meg a mentett konfigurációs fájl.</span><span class="sxs-lookup"><span data-stu-id="ae362-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="ae362-112">Ebben a példában a konfigurációs fájl neve Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="ae362-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="ae362-113">Az Office Deployment eszköz mód beállítása, és adja meg a konfigurációs fájlban.</span><span class="sxs-lookup"><span data-stu-id="ae362-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="ae362-114">**Megjegyzés:** Ebben a lépésben az ügyfélszámítógépről szeretné telepíteni az Office és helyi rendszergazdai jogosultságokkal kell rendelkeznie a számítógépen kell futtatni.</span><span class="sxs-lookup"><span data-stu-id="ae362-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="ae362-115">Az Office 365 ProPlus elképzelések Office telepítési eszköz használatával kapcsolatban további tudnivalókat [az Office telepítési eszköz – áttekintés](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="ae362-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="ae362-116">Az Office testreszabási eszközének használatáról további tudnivalókat talál [az Office testreszabási eszközének áttekintése](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="ae362-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

