---
title: Az Office 365 ProPlus telepítése az RDS, Terminal Server vagy VDI megosztott használatra
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959462"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Az Office 365 ProPlus telepítése az RDS, Terminal Server vagy VDI megosztott használatra

Az Office 365 ProPlus telepítése a távoli asztali szolgáltatásokkal (RDS), korábban Terminálszolgáltatások néven:
- Szükség van egy Microsoft 365 for Business tervre vagy egy Office 365 tervre, amely tartalmazza az Office 365 ProPlus programot, mint például az Office 365 Enterprise E3 vagy Enterprise E5.
   > [!NOTE] 
   > A Hivatal 365 teendő és Hivatal 365 teendő prémium tervek nem tartalmaz Hivatal 365 ProPlus.
- Engedélyeznie kell a [megosztott számítógép aktiválását](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Tudod is letölt és fuss a [Mikroszkóp támogat és visszaszerzés segéd](https://aka.ms/SaRA_OfficeSCA_M365Portal) -hoz felszerel hivatal 365 ProPlus-ban elosztva számítógép aktiválás mód.

A testreszabott telepítések előfeltételeiről, a telepítési utasításról és az Office központi telepítési eszköz használatával kapcsolatos útmutatásról az [office 365 ProPlus telepítése](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)című témakör nyújt bővebb felvilágosítást.

A megosztott számítógép-aktiválással kapcsolatos hibák kijavítása:
- További információ: az [Office 365 ProPlus esetében a megosztott számítógépes aktiválással kapcsolatos problémák elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Lásd: az [Office 365 ProPlus aktiválási állapotának visszaállítása](https://go.microsoft.com/fwlink/?linkid=2109218).

Ha ön akar-hoz felszerel hivatal 365 ProPlus-ra RDS-ból Mikroszkóp 365 admin központ, ***melyik használ hiba bevezetés elintézés***, használ a következő lép:

1.  Ellenőriz mi Hivatal 365 tervez Önnek van. [További információ](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Ha szükséges, váltson át egy másik Office 365-tervre. [További információ](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Ha az Office már telepítve van az RDS-kiszolgálón más Office 365-tervek használatával, távolítsa el azt. Például, mellett haladó **irányít tábla** > **uninstall egy műsor**. Eltávolítás a [Microsoft támogatási és helyreállítási segéd](https://aka.ms/SARA-OfficeUninstall-Alchemy) használatával, ha problémába fut.
4.  Az RDS-kiszolgálón jelentkezzen be a Microsoft 365 felügyeleti központba a rendszergazdai fiókkal, és telepítse az [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)programot.
5.  Az Office telepítését követően ***Ne nyisson meg és ne jelentkezzen be*** Office-alkalmazásokat.
6.  Az RDS-kiszolgálón a beállításjegyzék szerkesztésével engedélyezze a megosztott számítógép aktiválását az alábbi lépések végrehajtásával:
   1. Kattintson a jobb gombbal a képernyő bal alsó sarkában található Windows gombra, és válassza a **Futtatás**pontot. A Megnyitás mezőbe írja be a **Regedit**parancsot, majd kattintson az **OK gombra**.
   2. Ha a rendszer rákérdez, hogy engedélyezi-e a Rendszerleíróadatbázis-szerkesztőt az eszköz változtatásakor, válassza az **Igen** lehetőséget.
   3. A Rendszerleíróadatbázis-szerkesztőben adja hozzá a **Sharedcomputerlicensing** karakterlánc-értéket, amelynek beállítása 1 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Az RDS-kiszolgálón ***Jelentkezzen be végfelhasználóként*** , és ellenőrizze, [hogy a megosztott számítógép aktiválása engedélyezve van-e az Office 365 ProPlus esetében](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

