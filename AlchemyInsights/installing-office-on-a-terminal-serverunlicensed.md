---
title: A terminálkiszolgáló - nem licencelt office telepítése
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
ms.openlocfilehash: edac051840594f13b22ccd83f5cd6e3da5f84cbc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36498417"
---
# <a name="installing-office-on-a-terminal-server"></a>A terminálkiszolgálón futó Office telepítése

Találnak az Office 365 ProPlus a Windows Server távoli asztali szolgáltatások (RDS) segítségével, korábbi nevén a Terminálszolgáltatások:
  
- Az Office 365 terv, amely tartalmazza az Office 365 ProPlus, például az Office 365 vállalati E3 vagy vállalati E5 kell rendelkeznie. Az Office 365 üzleti és az Office 365 Business Premium tervek nem tartalmazzák az Office 365 ProPlus.

- [Megosztott számítógép-aktiválásnak](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)engedélyezni kell.

Ha a telepíteni kívánt Office 365 ProPlus a távoli asztali szolgáltatások az Office 365 Portal, ***alapértelmezett telepítési beállításokat használó***, kövesse az alábbi lépéseket:
  
1. Ellenőrizze, milyen Office 365 terv van. [Tájékoztatás arról, hogyan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Ha szükséges, váltson egy másik Office 365 tervezi. [Tájékoztatás arról, hogyan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Ha Office az RDS kiszolgáló használatával bármely más Office 365 tervek már telepítve van, távolítsa el azt. Például a Vezérlőpulton által \> távolítsa el a programot. Távolítsa el a problémák történő futtatása esetén használja a [Microsoft támogatási és helyreállítási Segéd](https://aka.ms/SARA-OfficeUninstall-Alchemy) .

4. A távoli asztali kiszolgálón jelentkezzen be a rendszergazdai fiókot, és [telepítse az Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)az Office 365 portálon.

5. Office telepítését követően ***Ne nyisson meg és jelentkezzen be*** minden Office alkalmazást.

6. A távoli asztali kiszolgálón engedélyezi a megosztott számítógép-aktiválás a rendszerleíró adatbázisban a következő lépések végrehajtásával:

1. Kattintson a jobb gombbal a Windows gombra a képernyő bal alsó sarkában, és válassza a Futtatás. A Megnyitás mezőbe írja be a **regedit parancsot**, és kattintson az OK gombra.

2. Válassza az Igen megjelenésekor a Rendszerleíróadatbázis-szerkesztő segítségével módosíthatja az eszköz.

3. A Rendszerleíróadatbázis-szerkesztő **SharedComputerLicensing** karakterlánc értéke 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration alapján adja hozzá.

7. Az RDS kiszolgáló, ***a felhasználó bejelentkezés*** és [Ellenőrizze, hogy a megosztott számítógép-aktiválásnak az Office 365 ProPlus van engedélyezve](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Előfeltételek, a telepítési utasításokat és útmutatást az Office telepítési eszköz segítségével testreszabott példányokat részletesebben lásd [Telepítése Office 365 ProPlus távoli asztali szolgáltatások használatával](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Megosztott számítógép-aktiválásnak kapcsolatos hibák elhárításához tanulmányozza [az Office 365 ProPlus megosztott számítógépen aktiválási problémák elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  