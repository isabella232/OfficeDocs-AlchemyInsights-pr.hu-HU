---
title: A terminálkiszolgáló - nem licencelt office telepítése
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29473587"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="eadcc-102">A terminálkiszolgálón futó Office telepítése</span><span class="sxs-lookup"><span data-stu-id="eadcc-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="eadcc-103">Találnak az Office 365 ProPlus a Windows Server távoli asztali szolgáltatások (RDS) segítségével, korábbi nevén a Terminálszolgáltatások:</span><span class="sxs-lookup"><span data-stu-id="eadcc-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="eadcc-p101">Az Office 365 terv, amely tartalmazza az Office 365 ProPlus, például az Office 365 vállalati E3 vagy vállalati E5 kell rendelkeznie. Az Office 365 üzleti és az Office 365 Business Premium tervek nem tartalmazzák az Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="eadcc-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="eadcc-106">[Megosztott számítógép-aktiválásnak](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)engedélyezni kell.</span><span class="sxs-lookup"><span data-stu-id="eadcc-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="eadcc-107">Ha a telepíteni kívánt Office 365 ProPlus a távoli asztali szolgáltatások az Office 365 Portal \*\* *alapértelmezett telepítési beállításokat használó* \*\*, kövesse az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="eadcc-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="eadcc-p102">Ellenőrizze, milyen Office 365 terv van. [Megtudhatja, hogyan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="eadcc-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="eadcc-p103">Ha szükséges, váltson egy másik Office 365 tervezi. [Megtudhatja, hogyan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="eadcc-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="eadcc-p104">Ha Office az RDS kiszolgáló használatával bármely más Office 365 tervek már telepítve van, távolítsa el azt. Például a Vezérlőpulton által \> távolítsa el a programot. Távolítsa el a problémák történő futtatása esetén használja a [Microsoft támogatási és helyreállítási Segéd](https://aka.ms/SARA-OfficeUninstall-Alchemy) .</span><span class="sxs-lookup"><span data-stu-id="eadcc-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="eadcc-115">A távoli asztali kiszolgálón jelentkezzen be a rendszergazdai fiókot, és [telepítse az Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)az Office 365 portálon.</span><span class="sxs-lookup"><span data-stu-id="eadcc-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="eadcc-116">Office telepítése után \*\* *Ne nyisson meg és jelentkezzen be* \*\* bármely Office-alkalmazásokkal.</span><span class="sxs-lookup"><span data-stu-id="eadcc-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="eadcc-117">A távoli asztali kiszolgálón engedélyezi a megosztott számítógép-aktiválás a rendszerleíró adatbázisban a következő lépések végrehajtásával:</span><span class="sxs-lookup"><span data-stu-id="eadcc-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="eadcc-p105">Kattintson a jobb gombbal a Windows gombra a képernyő bal alsó sarkában, és válassza a Futtatás. A Megnyitás mezőbe írja be a **regedit parancsot**, és kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="eadcc-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="eadcc-120">Válassza az Igen megjelenésekor a Rendszerleíróadatbázis-szerkesztő segítségével módosíthatja az eszköz.</span><span class="sxs-lookup"><span data-stu-id="eadcc-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="eadcc-121">A Rendszerleíróadatbázis-szerkesztő **SharedComputerLicensing** karakterlánc értéke 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration alapján adja hozzá.</span><span class="sxs-lookup"><span data-stu-id="eadcc-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="eadcc-122">A távoli asztali kiszolgálón \*\* *a felhasználó bejelentkezés* \*\*, és [Ellenőrizze, hogy a megosztott számítógép-aktiválásnak engedélyezve van az Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="eadcc-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="eadcc-123">Előfeltételek, a telepítési utasításokat és útmutatást az Office telepítési eszköz segítségével testreszabott példányokat részletesebben lásd [Telepítése Office 365 ProPlus távoli asztali szolgáltatások használatával](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="eadcc-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="eadcc-124">Megosztott számítógép-aktiválásnak kapcsolatos hibák elhárításához tanulmányozza [az Office 365 ProPlus megosztott számítógépen aktiválási problémák elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="eadcc-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

