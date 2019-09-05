---
title: Office telepítése terminálkiszolgálón-nem licencelt
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735391"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="12b3a-102">Az Office telepítése terminálkiszolgálón</span><span class="sxs-lookup"><span data-stu-id="12b3a-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="12b3a-103">Az Office 365 ProPlus egy Windows Server rendszerben, a távoli asztali szolgáltatásokkal (RDS), korábban Terminálszolgáltatások néven történő telepítésével.</span><span class="sxs-lookup"><span data-stu-id="12b3a-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="12b3a-104">Rendelkeznie kell egy Office 365 terv, amely tartalmazza az Office 365 ProPlus, mint például az Office 365 Enterprise E3 vagy Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="12b3a-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="12b3a-105">A Hivatal 365 teendő és Hivatal 365 teendő prémium tervek nem tartalmaz Hivatal 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="12b3a-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="12b3a-106">Engedélyeznie kell a [megosztott számítógép aktiválását](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="12b3a-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="12b3a-107">Ha ön akar-hoz felszerel hivatal 365 ProPlus-ra RDS-ból Mikroszkóp 365 admin központ, ***melyik használ hiba bevezetés elintézés***, követ ezek lép:</span><span class="sxs-lookup"><span data-stu-id="12b3a-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="12b3a-108">Ellenőriz mi Hivatal 365 tervez Önnek van.</span><span class="sxs-lookup"><span data-stu-id="12b3a-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="12b3a-109">Ismerje meg, hogyan</span><span class="sxs-lookup"><span data-stu-id="12b3a-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="12b3a-110">Ha szükséges, váltson át egy másik Office 365-tervre.</span><span class="sxs-lookup"><span data-stu-id="12b3a-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="12b3a-111">Ismerje meg, hogyan</span><span class="sxs-lookup"><span data-stu-id="12b3a-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="12b3a-112">Ha az Office már telepítve van az RDS-kiszolgálón más Office 365-tervek használatával, távolítsa el azt.</span><span class="sxs-lookup"><span data-stu-id="12b3a-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="12b3a-113">Például, mellett haladó irányít tábla \> uninstall egy műsor.</span><span class="sxs-lookup"><span data-stu-id="12b3a-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="12b3a-114">Eltávolítás a [Microsoft támogatási és helyreállítási segéd](https://aka.ms/SARA-OfficeUninstall-Alchemy) használatával, ha problémába fut.</span><span class="sxs-lookup"><span data-stu-id="12b3a-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="12b3a-115">Az RDS-kiszolgálón jelentkezzen be a Microsoft 365 felügyeleti központba a rendszergazdai fiókkal, és telepítse az [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)programot.</span><span class="sxs-lookup"><span data-stu-id="12b3a-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="12b3a-116">Az Office telepítését követően ***Ne nyisson meg és ne jelentkezzen be*** Office-alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="12b3a-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="12b3a-117">Az RDS-kiszolgálón a beállításjegyzék szerkesztésével engedélyezze a megosztott számítógép aktiválását az alábbi lépések végrehajtásával:</span><span class="sxs-lookup"><span data-stu-id="12b3a-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="12b3a-118">Kattintson a jobb gombbal a képernyő bal alsó sarkában található Windows gombra, és válassza a Futtatás pontot.</span><span class="sxs-lookup"><span data-stu-id="12b3a-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="12b3a-119">A Megnyitás mezőbe írja be a **Regedit**parancsot, majd kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="12b3a-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="12b3a-120">Amikor a rendszer megkérdezi, hogy engedélyezi-e a Rendszerleíróadatbázis-szerkesztőt az eszköz változtatásakor, válassza az Igen beállítást.</span><span class="sxs-lookup"><span data-stu-id="12b3a-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="12b3a-121">A Rendszerleíróadatbázis-szerkesztőben adja hozzá a **Sharedcomputerlicensing** karakterlánc-értéket, amelynek beállítása 1, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="12b3a-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="12b3a-122">Az RDS-kiszolgálón ***Jelentkezzen be végfelhasználóként*** , és ellenőrizze, [hogy a megosztott számítógép aktiválása engedélyezve van-e az Office 365 ProPlus esetében](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="12b3a-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="12b3a-123">Ha többet kíván megtudni az előfeltételekről, a telepítési utasításról és a testreszabott telepítések útmutatásával kapcsolatban az Office Deployment Tool alkalmazással, olvassa el az [office 365 ProPlus telepítése című témakört a távoli asztali szolgáltatások segítségével](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="12b3a-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="12b3a-124">A megosztott számítógép-aktiválással kapcsolatos hibák kijavításához tekintse meg [az Office 365 ProPlus számítógép-aktiválási problémáinak elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)című témakört.</span><span class="sxs-lookup"><span data-stu-id="12b3a-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  