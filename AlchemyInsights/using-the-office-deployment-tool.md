---
title: Az Office-telepítő eszköz használata
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794913"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="01f3b-102">Az Office-telepítő eszköz használata (ODT)</span><span class="sxs-lookup"><span data-stu-id="01f3b-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="01f3b-103">Az Office-telepítő eszköz (ODT) segítségével telepítheti az Office 365 Office-verzióit.</span><span class="sxs-lookup"><span data-stu-id="01f3b-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="01f3b-104">Az Office-telepítő eszköz (setup.exe) a parancssorból futtatható, és egy konfigurációs XML-fájlt használ annak meghatározásához, hogy milyen beállítások vonatkoznak az Office telepítésekor.</span><span class="sxs-lookup"><span data-stu-id="01f3b-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="01f3b-105">Töltse le az Office-telepítő eszköz legújabb verzióját a [Microsoft letöltőközpontból](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="01f3b-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="01f3b-106">Az [Office customization Tool (TOT)](https://config.office.com) segítségével jelölje ki a központi telepítő beállításait, és hozza létre a konfigurációs XML-fájlt.</span><span class="sxs-lookup"><span data-stu-id="01f3b-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="01f3b-107">Exportálja a konfigurációs fájlt, és helyezze azt helyileg ugyanarra a mappába, ahol a setup.exe található.</span><span class="sxs-lookup"><span data-stu-id="01f3b-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="01f3b-108">**Megjegyzés:** Az Office telepítési problémái gyakran előfordulnak a helytelenül konfigurált vagy malformatted konfigurációs fájlok miatt.</span><span class="sxs-lookup"><span data-stu-id="01f3b-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="01f3b-109">Az ilyen problémák elkerülése érdekében az Office customization Tool segítségével hozza létre a konfigurációs fájlt.</span><span class="sxs-lookup"><span data-stu-id="01f3b-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="01f3b-110">A meglévő konfigurációs fájlokat is importálhatja az Office customization Tool alkalmazásba.</span><span class="sxs-lookup"><span data-stu-id="01f3b-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="01f3b-111">Egy rendszergazdai jogú parancssorból váltson arra a helyre, ahol a setup.exe-ban lakik, és futtassa az Office-telepítő eszközt a letöltési módban, és adja meg az imént mentett konfigurációs fájlt.</span><span class="sxs-lookup"><span data-stu-id="01f3b-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="01f3b-112">Ebben a példában a konfigurációs fájl neve Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="01f3b-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setup.exe /download Configuration.xml```

<span data-ttu-id="01f3b-113">4. Futtassa az Office-telepítő eszközt a konfigurálás módban, és adja meg a konfigurációs fájlt.</span><span class="sxs-lookup"><span data-stu-id="01f3b-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setup.exe /configure Configuration.xml```

<span data-ttu-id="01f3b-114">**Megjegyzés:** Ezt a lépést az ügyfélgépről kell futtatnia, amelyen telepíteni szeretné az Office-t, és a számítógépen helyi rendszergazdai engedélyekkel kell rendelkeznie.</span><span class="sxs-lookup"><span data-stu-id="01f3b-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="01f3b-115">Ha többet szeretne tudni az Office-telepítő eszköz használatáról a Microsoft 365-alkalmazásaiban a nagyvállalati telepítéshez, olvassa el [az Office-telepítő eszköz áttekintése](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)című témakört.</span><span class="sxs-lookup"><span data-stu-id="01f3b-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="01f3b-116">Az Office customization Tool használatáról további információt [az Office customization Tool áttekintése](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="01f3b-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
