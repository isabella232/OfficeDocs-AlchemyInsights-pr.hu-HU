---
title: Az Office telepítése terminálkiszolgálón – licenccel nem rendelkezők
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663119"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="33534-102">Az Office telepítése terminálkiszolgálóra</span><span class="sxs-lookup"><span data-stu-id="33534-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="33534-103">A Microsoft 365-alkalmazások nagyvállalati verzióra történő központi telepítése Windows Server rendszerű távoli asztali szolgáltatásokkal (RDS), korábbi nevén Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="33534-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="33534-104">Rendelkeznie kell egy olyan Microsoft 365-előfizetéssel, amely tartalmazza a nagyvállalati Microsoft 365-alkalmazásokat, például az Office 365 Enterprise E3 vagy a nagyvállalati E5 csomagját.</span><span class="sxs-lookup"><span data-stu-id="33534-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="33534-105">A Microsoft 365-alkalmazások vállalati verzió és a Microsoft 365-alkalmazások vállalati prémium verzióra szóló csomagja nem tartalmazza a Microsoft 365-alkalmazásokat a nagyvállalatoknak.</span><span class="sxs-lookup"><span data-stu-id="33534-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="33534-106">Engedélyeznie kell a [megosztott számítógép aktiválását](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="33534-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="33534-107">Ha a Microsoft 365-alkalmazásokat a nagyvállalati verzióra szeretné telepíteni a Microsoft 365 felügyeleti központból, ***amely az alapértelmezett telepítési beállításokat használja***, kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="33534-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="33534-108">Azt is megteheti, hogy letölti és futtatja a [Microsoft támogatási és helyreállítási Segédet](https://aka.ms/SaRA_OfficeSCA_M365Portal) a Microsoft 365-alkalmazások nagyvállalatoknak való telepítéséhez a megosztott számítógép-aktiválási módban.</span><span class="sxs-lookup"><span data-stu-id="33534-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="33534-109">Ellenőrizze, hogy melyik Microsoft 365-előfizetéssel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="33534-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="33534-110">További információ</span><span class="sxs-lookup"><span data-stu-id="33534-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="33534-111">Ha szükséges, váltson át egy másik Microsoft 365-előfizetésre.</span><span class="sxs-lookup"><span data-stu-id="33534-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="33534-112">További információ</span><span class="sxs-lookup"><span data-stu-id="33534-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="33534-113">Ha az Office már telepítve van az RDS-kiszolgálón bármely más Microsoft 365-előfizetéssel, távolítsa el.</span><span class="sxs-lookup"><span data-stu-id="33534-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="33534-114">Ha például a Vezérlőpultot fogja használni, \> távolítsa el a programot.</span><span class="sxs-lookup"><span data-stu-id="33534-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="33534-115">Ha problémákat tapasztal, távolítsa el a [Microsoft támogatási és helyreállítási Segédet](https://aka.ms/SARA-OfficeUninstall-Alchemy) .</span><span class="sxs-lookup"><span data-stu-id="33534-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="33534-116">Az RDS-kiszolgálón bejelentkezés a Microsoft 365 felügyeleti központba a rendszergazdai fiókjával és a [microsoft 365-alkalmazások telepítése nagyvállalati](https://portal.office.com/OLS/MySoftware.aspx)verzióba.</span><span class="sxs-lookup"><span data-stu-id="33534-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="33534-117">Miután telepítette az Office-t, ***Ne nyisson meg vagy ne írjon be*** semmilyen Office-alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="33534-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="33534-118">Az RDS-kiszolgálón engedélyezze a megosztott számítógép-aktiválást a beállításjegyzék szerkesztésével a következő lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="33534-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="33534-119">Kattintson a jobb gombbal a Windows gombra a képernyő bal alsó sarkában, és válassza a Futtatás parancsot.</span><span class="sxs-lookup"><span data-stu-id="33534-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="33534-120">A Megnyitás mezőbe írja be a **Regedit szót**, majd válassza az OK gombot.</span><span class="sxs-lookup"><span data-stu-id="33534-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="33534-121">Ha a rendszer kéri, válassza az Igen lehetőséget, ha az eszközén módosítani szeretné a beállításszerkesztőt.</span><span class="sxs-lookup"><span data-stu-id="33534-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="33534-122">A Rendszerleíróadatbázis-szerkesztőben adjon meg egy karakterláncot az **SharedComputerLicensing** , amelynek értéke 1 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="33534-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="33534-123">Az RDS-kiszolgálón a ***Bejelentkezés végfelhasználóként*** , és [ellenőrizze, hogy engedélyezve van-e a Microsoft 365-alkalmazások nagyvállalatoknak való aktiválása a megosztott számítógépeken](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="33534-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="33534-124">Ha további információra van kíváncsi a testreszabott példányokra vonatkozó előfeltételekről és útmutatásról az Office-telepítő eszközzel, olvassa el a [Microsoft 365-alkalmazások telepítése nagyvállalatoknak a távoli asztali szolgáltatások segítségével](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)című témakört.</span><span class="sxs-lookup"><span data-stu-id="33534-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="33534-125">A megosztott számítógép-aktiválással kapcsolatos hibák [elhárításáról a Microsoft 365-alkalmazások a nagyvállalati verzióhoz készült aktiválással kapcsolatos problémák elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)című témakörben talál további tájékoztatást.</span><span class="sxs-lookup"><span data-stu-id="33534-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  