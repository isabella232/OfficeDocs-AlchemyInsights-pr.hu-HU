---
title: Office telepítése terminálkiszolgálón-nem licencelt
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205411"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="6ab16-102">Az Office telepítése terminálkiszolgálón</span><span class="sxs-lookup"><span data-stu-id="6ab16-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="6ab16-103">Az Office 365 ProPlus egy Windows Server rendszerben, a távoli asztali szolgáltatásokkal (RDS), korábban Terminálszolgáltatások néven történő telepítésével.</span><span class="sxs-lookup"><span data-stu-id="6ab16-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="6ab16-104">Rendelkeznie kell egy Office 365 terv, amely tartalmazza az Office 365 ProPlus, mint például az Office 365 Enterprise E3 vagy Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="6ab16-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="6ab16-105">A Hivatal 365 teendő és Hivatal 365 teendő prémium tervek nem tartalmaz Hivatal 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="6ab16-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="6ab16-106">Engedélyeznie kell a [megosztott számítógép aktiválását](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="6ab16-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="6ab16-107">Ha ön akar-hoz felszerel hivatal 365 ProPlus-ra RDS-ból Mikroszkóp 365 admin központ, ***melyik használ hiba bevezetés elintézés***, használ a következő lép.</span><span class="sxs-lookup"><span data-stu-id="6ab16-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="6ab16-108">Tudod is letölt és fuss a [Mikroszkóp támogat és visszaszerzés segéd](https://aka.ms/SaRA_OfficeSCA_M365Portal) -hoz felszerel hivatal 365 ProPlus-ban elosztva számítógép aktiválás mód.</span><span class="sxs-lookup"><span data-stu-id="6ab16-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="6ab16-109">Ellenőriz mi Hivatal 365 tervez Önnek van.</span><span class="sxs-lookup"><span data-stu-id="6ab16-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="6ab16-110">Ismerje meg, hogyan</span><span class="sxs-lookup"><span data-stu-id="6ab16-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="6ab16-111">Ha szükséges, váltson át egy másik Office 365-tervre.</span><span class="sxs-lookup"><span data-stu-id="6ab16-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="6ab16-112">Ismerje meg, hogyan</span><span class="sxs-lookup"><span data-stu-id="6ab16-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="6ab16-113">Ha az Office már telepítve van az RDS-kiszolgálón más Office 365-tervek használatával, távolítsa el azt.</span><span class="sxs-lookup"><span data-stu-id="6ab16-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="6ab16-114">Például, mellett haladó irányít tábla \> uninstall egy műsor.</span><span class="sxs-lookup"><span data-stu-id="6ab16-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="6ab16-115">Eltávolítás a [Microsoft támogatási és helyreállítási segéd](https://aka.ms/SARA-OfficeUninstall-Alchemy) használatával, ha problémába fut.</span><span class="sxs-lookup"><span data-stu-id="6ab16-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="6ab16-116">Az RDS-kiszolgálón jelentkezzen be a Microsoft 365 felügyeleti központba a rendszergazdai fiókkal, és telepítse az [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)programot.</span><span class="sxs-lookup"><span data-stu-id="6ab16-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="6ab16-117">Az Office telepítését követően ***Ne nyisson meg és ne jelentkezzen be*** Office-alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="6ab16-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="6ab16-118">Az RDS-kiszolgálón a beállításjegyzék szerkesztésével engedélyezze a megosztott számítógép aktiválását az alábbi lépések végrehajtásával:</span><span class="sxs-lookup"><span data-stu-id="6ab16-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="6ab16-119">Kattintson a jobb gombbal a képernyő bal alsó sarkában található Windows gombra, és válassza a Futtatás pontot.</span><span class="sxs-lookup"><span data-stu-id="6ab16-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="6ab16-120">A Megnyitás mezőbe írja be a **Regedit**parancsot, majd kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="6ab16-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="6ab16-121">Amikor a rendszer megkérdezi, hogy engedélyezi-e a Rendszerleíróadatbázis-szerkesztőt az eszköz változtatásakor, válassza az Igen beállítást.</span><span class="sxs-lookup"><span data-stu-id="6ab16-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="6ab16-122">A Rendszerleíróadatbázis-szerkesztőben adja hozzá a **Sharedcomputerlicensing** karakterlánc-értéket, amelynek beállítása 1, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="6ab16-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="6ab16-123">Az RDS-kiszolgálón ***Jelentkezzen be végfelhasználóként*** , és ellenőrizze, [hogy a megosztott számítógép aktiválása engedélyezve van-e az Office 365 ProPlus esetében](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="6ab16-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="6ab16-124">Ha többet kíván megtudni az előfeltételekről, a telepítési utasításról és a testreszabott telepítések útmutatásával kapcsolatban az Office Deployment Tool alkalmazással, olvassa el az [office 365 ProPlus telepítése című témakört a távoli asztali szolgáltatások segítségével](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="6ab16-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="6ab16-125">A megosztott számítógép-aktiválással kapcsolatos hibák kijavításához tekintse meg [az Office 365 ProPlus számítógép-aktiválási problémáinak elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)című témakört.</span><span class="sxs-lookup"><span data-stu-id="6ab16-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  