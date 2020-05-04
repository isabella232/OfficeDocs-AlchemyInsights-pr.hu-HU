---
title: Az Office-telepítő eszköz használata
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: d941bce524dc797d5dcbb7213bded6919fd01b7d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010868"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="8a8c1-102">Az Office-telepítő eszköz (ODT) használata</span><span class="sxs-lookup"><span data-stu-id="8a8c1-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="8a8c1-103">Az Office-telepítő eszközzel (ODT) telepítheti az Office 365 Office-verzióit.</span><span class="sxs-lookup"><span data-stu-id="8a8c1-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="8a8c1-104">Az Office deployment tool (setup.exe) parancssorból fut, és egy konfigurációs XML-fájl segítségével határozza meg, hogy milyen beállításokat kell alkalmazni az Office telepítésekor.</span><span class="sxs-lookup"><span data-stu-id="8a8c1-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="8a8c1-105">Töltse le az Office telepítőeszköz legújabb verzióját a [Microsoft letöltőközpontjából.](https://go.microsoft.com/fwlink/p/?LinkID=626065)</span><span class="sxs-lookup"><span data-stu-id="8a8c1-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="8a8c1-106">Az [Office testreszabási eszközével (OCT)](https://config.office.com) kiválaszthatja a telepítési beállításokat, és létrehozhatja a konfigurációs XML-fájlt.</span><span class="sxs-lookup"><span data-stu-id="8a8c1-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="8a8c1-107">Exportálja a konfigurációs fájlt, és helyezze helyileg ugyanarra a mappára, ahol a setup.exe található.</span><span class="sxs-lookup"><span data-stu-id="8a8c1-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="8a8c1-108">**Megjegyzés:** Az Office telepítésével kapcsolatos problémák gyakran a helytelenül konfigurált vagy helytelenül formázott konfigurációs fájlok miatt jelentkeznek.</span><span class="sxs-lookup"><span data-stu-id="8a8c1-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="8a8c1-109">Az ilyen problémák elkerülése érdekében javasoljuk, hogy az Office testreszabási eszközével hozza létre a konfigurációs fájlt.</span><span class="sxs-lookup"><span data-stu-id="8a8c1-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="8a8c1-110">Meglévő konfigurációs fájlokat is importálhat az Office testreszabási eszközébe.</span><span class="sxs-lookup"><span data-stu-id="8a8c1-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="8a8c1-111">A rendszergazda jogú parancssorból váltson arra a helyre, ahol a setup.exe található, és futtassa az Office-telepítési eszközt letöltési módban, és adja meg az imént mentett konfigurációs fájlt.</span><span class="sxs-lookup"><span data-stu-id="8a8c1-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="8a8c1-112">Ebben a példában a konfigurációs fájl neve Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="8a8c1-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="8a8c1-113">Futtassa az Office-telepítő eszközt konfigurálási módban, és adja meg a konfigurációs fájlt.</span><span class="sxs-lookup"><span data-stu-id="8a8c1-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="8a8c1-114">**Megjegyzés:** Ezt a lépést arról az ügyfélszámítógépről kell futtatnia, amelyre telepíteni szeretné az Office-t, és helyi rendszergazdai engedélyekkel kell rendelkeznie a számítógépen.</span><span class="sxs-lookup"><span data-stu-id="8a8c1-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="8a8c1-115">Ha többet szeretne tudni arról, hogy miként használható az Office-telepítő eszköz a Microsoft 365-alkalmazásokhoz vállalati telepítési helyzetekben, olvassa [el az Office-telepítési eszköz áttekintése című témakört.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)</span><span class="sxs-lookup"><span data-stu-id="8a8c1-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="8a8c1-116">Az Office testreszabási eszközének használatáról az [Office testreszabási eszköz áttekintése című témakörben olvashat bővebben.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)</span><span class="sxs-lookup"><span data-stu-id="8a8c1-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
