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
# <a name="installing-office-on-a-terminal-server"></a>Az Office telepítése terminálkiszolgálón

Az Office 365 ProPlus egy Windows Server rendszerben, a távoli asztali szolgáltatásokkal (RDS), korábban Terminálszolgáltatások néven történő telepítésével.
  
- Rendelkeznie kell egy Office 365 terv, amely tartalmazza az Office 365 ProPlus, mint például az Office 365 Enterprise E3 vagy Enterprise E5. A Hivatal 365 teendő és Hivatal 365 teendő prémium tervek nem tartalmaz Hivatal 365 ProPlus.

- Engedélyeznie kell a [megosztott számítógép aktiválását](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Ha ön akar-hoz felszerel hivatal 365 ProPlus-ra RDS-ból Mikroszkóp 365 admin központ, ***melyik használ hiba bevezetés elintézés***, használ a következő lép.

> [!TIP]
> Tudod is letölt és fuss a [Mikroszkóp támogat és visszaszerzés segéd](https://aka.ms/SaRA_OfficeSCA_M365Portal) -hoz felszerel hivatal 365 ProPlus-ban elosztva számítógép aktiválás mód.
  
1. Ellenőriz mi Hivatal 365 tervez Önnek van. [Ismerje meg, hogyan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Ha szükséges, váltson át egy másik Office 365-tervre. [Ismerje meg, hogyan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Ha az Office már telepítve van az RDS-kiszolgálón más Office 365-tervek használatával, távolítsa el azt. Például, mellett haladó irányít tábla \> uninstall egy műsor. Eltávolítás a [Microsoft támogatási és helyreállítási segéd](https://aka.ms/SARA-OfficeUninstall-Alchemy) használatával, ha problémába fut.

4. Az RDS-kiszolgálón jelentkezzen be a Microsoft 365 felügyeleti központba a rendszergazdai fiókkal, és telepítse az [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)programot.

5. Az Office telepítését követően ***Ne nyisson meg és ne jelentkezzen be*** Office-alkalmazásokat.

6. Az RDS-kiszolgálón a beállításjegyzék szerkesztésével engedélyezze a megosztott számítógép aktiválását az alábbi lépések végrehajtásával:

1. Kattintson a jobb gombbal a képernyő bal alsó sarkában található Windows gombra, és válassza a Futtatás pontot. A Megnyitás mezőbe írja be a **Regedit**parancsot, majd kattintson az OK gombra.

2. Amikor a rendszer megkérdezi, hogy engedélyezi-e a Rendszerleíróadatbázis-szerkesztőt az eszköz változtatásakor, válassza az Igen beállítást.

3. A Rendszerleíróadatbázis-szerkesztőben adja hozzá a **Sharedcomputerlicensing** karakterlánc-értéket, amelynek beállítása 1, HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Az RDS-kiszolgálón ***Jelentkezzen be végfelhasználóként*** , és ellenőrizze, [hogy a megosztott számítógép aktiválása engedélyezve van-e az Office 365 ProPlus esetében](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Ha többet kíván megtudni az előfeltételekről, a telepítési utasításról és a testreszabott telepítések útmutatásával kapcsolatban az Office Deployment Tool alkalmazással, olvassa el az [office 365 ProPlus telepítése című témakört a távoli asztali szolgáltatások segítségével](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
A megosztott számítógép-aktiválással kapcsolatos hibák kijavításához tekintse meg [az Office 365 ProPlus számítógép-aktiválási problémáinak elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)című témakört.
  