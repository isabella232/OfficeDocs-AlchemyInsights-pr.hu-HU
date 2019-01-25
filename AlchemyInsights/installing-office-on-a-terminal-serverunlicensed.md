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
# <a name="installing-office-on-a-terminal-server"></a>A terminálkiszolgálón futó Office telepítése

Találnak az Office 365 ProPlus a Windows Server távoli asztali szolgáltatások (RDS) segítségével, korábbi nevén a Terminálszolgáltatások:
  
- Az Office 365 terv, amely tartalmazza az Office 365 ProPlus, például az Office 365 vállalati E3 vagy vállalati E5 kell rendelkeznie. Az Office 365 üzleti és az Office 365 Business Premium tervek nem tartalmazzák az Office 365 ProPlus.
    
- [Megosztott számítógép-aktiválásnak](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)engedélyezni kell.
    
Ha a telepíteni kívánt Office 365 ProPlus a távoli asztali szolgáltatások az Office 365 Portal ** *alapértelmezett telepítési beállításokat használó* **, kövesse az alábbi lépéseket: 
  
1. Ellenőrizze, milyen Office 365 terv van. [Megtudhatja, hogyan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Ha szükséges, váltson egy másik Office 365 tervezi. [Megtudhatja, hogyan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Ha Office az RDS kiszolgáló használatával bármely más Office 365 tervek már telepítve van, távolítsa el azt. Például a Vezérlőpulton által \> távolítsa el a programot. Távolítsa el a problémák történő futtatása esetén használja a [Microsoft támogatási és helyreállítási Segéd](https://aka.ms/SARA-OfficeUninstall-Alchemy) . 
    
4. A távoli asztali kiszolgálón jelentkezzen be a rendszergazdai fiókot, és [telepítse az Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)az Office 365 portálon.
    
5. Office telepítése után ** *Ne nyisson meg és jelentkezzen be* ** bármely Office-alkalmazásokkal. 
    
6. A távoli asztali kiszolgálón engedélyezi a megosztott számítógép-aktiválás a rendszerleíró adatbázisban a következő lépések végrehajtásával:
    
1. Kattintson a jobb gombbal a Windows gombra a képernyő bal alsó sarkában, és válassza a Futtatás. A Megnyitás mezőbe írja be a **regedit parancsot**, és kattintson az OK gombra. 
    
2. Válassza az Igen megjelenésekor a Rendszerleíróadatbázis-szerkesztő segítségével módosíthatja az eszköz.
    
3. A Rendszerleíróadatbázis-szerkesztő **SharedComputerLicensing** karakterlánc értéke 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration alapján adja hozzá. 
    
7. A távoli asztali kiszolgálón ** *a felhasználó bejelentkezés* **, és [Ellenőrizze, hogy a megosztott számítógép-aktiválásnak engedélyezve van az Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Előfeltételek, a telepítési utasításokat és útmutatást az Office telepítési eszköz segítségével testreszabott példányokat részletesebben lásd [Telepítése Office 365 ProPlus távoli asztali szolgáltatások használatával](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Megosztott számítógép-aktiválásnak kapcsolatos hibák elhárításához tanulmányozza [az Office 365 ProPlus megosztott számítógépen aktiválási problémák elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

