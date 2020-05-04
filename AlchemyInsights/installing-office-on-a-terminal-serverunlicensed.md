---
title: Az iroda telepítése terminálkiszolgálón – Nem licencelt
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
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010616"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="5fbfb-102">Az Office telepítése terminálkiszolgálóra</span><span class="sxs-lookup"><span data-stu-id="5fbfb-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="5fbfb-103">Microsoft 365-alkalmazások vállalati telepítéséhez Windows Server en a Távoli asztali szolgáltatások (RDS) használatával, amelyet korábbi nevén Terminálszolgáltatások nak neveztek el:</span><span class="sxs-lookup"><span data-stu-id="5fbfb-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="5fbfb-104">Olyan Microsoft 365-előfizetéssel kell rendelkeznie, amely tartalmazza a nagyvállalati Microsoft 365 alkalmazásokat, például az Office 365 Nagyvállalati E3 vagy nagyvállalati E5 verziót.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="5fbfb-105">A Microsoft 365 vállalati alkalmazások és a Microsoft 365 Apps for Business Premium csomagok nem tartalmazzák a nagyvállalati Microsoft 365 alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="5fbfb-106">Engedélyeznie kell a [megosztott számítógép aktiválását.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="5fbfb-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="5fbfb-107">Ha a Microsoft 365 vállalati alkalmazásokat az RDS szolgáltatásba szeretné telepíteni a Microsoft 365 Felügyeleti központból, ***amely az alapértelmezett telepítési beállításokat használja,*** kövesse az alábbi lépéseket.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="5fbfb-108">A [Microsoft támogatási és helyreállítási segédjét](https://aka.ms/SaRA_OfficeSCA_M365Portal) is letöltheti és futtathatja a Microsoft 365 vállalati alkalmazások megosztott számítógép-aktiválási módban történő telepítéséhez.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="5fbfb-109">Ellenőrizze, hogy milyen Microsoft 365-előfizetéssel rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="5fbfb-110">Ismerje meg, hogyan</span><span class="sxs-lookup"><span data-stu-id="5fbfb-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="5fbfb-111">Szükség esetén váltson másik Microsoft 365-előfizetésre.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="5fbfb-112">Ismerje meg, hogyan</span><span class="sxs-lookup"><span data-stu-id="5fbfb-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="5fbfb-113">Ha az Office már telepítve van az RDS-kiszolgálón bármely más Microsoft 365-előfizetéssel, távolítsa el azt.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="5fbfb-114">Például a Vezérlőpult \> eltávolítása parancsra.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="5fbfb-115">Eltávolítás a [Microsoft támogatási és helyreállítási segédsegítségével,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ha problémákba ütközik.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="5fbfb-116">Az RDS-kiszolgálón jelentkezzen be a Microsoft 365 felügyeleti központba a rendszergazdai fiókkal, és [telepítse a Microsoft 365 vállalati alkalmazásokat.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="5fbfb-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="5fbfb-117">Az Office telepítése után ***ne nyisson meg és ne jelentkezzen be*** egyetlen Office-alkalmazásba sem.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="5fbfb-118">Az RDS-kiszolgálón engedélyezze a megosztott számítógép aktiválását a rendszerleíró adatbázis szerkesztésével az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="5fbfb-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="5fbfb-119">Kattintson a jobb gombbal a képernyő bal alsó sarkában lévő Windows gombra, és válassza a Futtatás parancsot.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="5fbfb-120">A Megnyitás mezőbe írja be a **regedit parancsot,** majd kattintson az OK gombra.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="5fbfb-121">Válassza az Igen lehetőséget, amikor a rendszer kéri, hogy a Rendszerleíróadatbázis-szerkesztő módosíthassa az eszközt.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="5fbfb-122">A Beállításjegyzék-szerkesztőben adjon meg egy **SharedComputerLicensing** karakterlánc-értéket 1-es értékkel a HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration csoportban.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="5fbfb-123">Az RDS-kiszolgálón ***jelentkezzen be végfelhasználóként,*** és [ellenőrizze, hogy a microsoft 365-ös vállalati alkalmazások esetében engedélyezve van-e a megosztott számítógép aktiválása.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="5fbfb-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="5fbfb-124">Az előfeltételekről, a telepítési utasításokról és a testreszabott telepítésekkel kapcsolatos útmutatásról az Office központi telepítési eszközével a [Microsoft 365-alkalmazások telepítése nagyvállalatoknak a Távoli asztali szolgáltatások használatával](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)című témakörben talál további információt.</span><span class="sxs-lookup"><span data-stu-id="5fbfb-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="5fbfb-125">A megosztott számítógép-aktiválással kapcsolatos hibák kijavításáról olvassa el A [Microsoft 365 vállalati alkalmazások megosztott számítógép-aktiválásával kapcsolatos problémák elhárítása című témakört.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="5fbfb-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  