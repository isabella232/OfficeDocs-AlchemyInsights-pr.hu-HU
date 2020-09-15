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
# <a name="installing-office-on-a-terminal-server"></a>Az Office telepítése terminálkiszolgálóra

A Microsoft 365-alkalmazások nagyvállalati verzióra történő központi telepítése Windows Server rendszerű távoli asztali szolgáltatásokkal (RDS), korábbi nevén Terminal Services:
  
- Rendelkeznie kell egy olyan Microsoft 365-előfizetéssel, amely tartalmazza a nagyvállalati Microsoft 365-alkalmazásokat, például az Office 365 Enterprise E3 vagy a nagyvállalati E5 csomagját. A Microsoft 365-alkalmazások vállalati verzió és a Microsoft 365-alkalmazások vállalati prémium verzióra szóló csomagja nem tartalmazza a Microsoft 365-alkalmazásokat a nagyvállalatoknak.

- Engedélyeznie kell a [megosztott számítógép aktiválását](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ha a Microsoft 365-alkalmazásokat a nagyvállalati verzióra szeretné telepíteni a Microsoft 365 felügyeleti központból, ***amely az alapértelmezett telepítési beállításokat használja***, kövesse az alábbi lépéseket.

> [!TIP]
> Azt is megteheti, hogy letölti és futtatja a [Microsoft támogatási és helyreállítási Segédet](https://aka.ms/SaRA_OfficeSCA_M365Portal) a Microsoft 365-alkalmazások nagyvállalatoknak való telepítéséhez a megosztott számítógép-aktiválási módban.
  
1. Ellenőrizze, hogy melyik Microsoft 365-előfizetéssel rendelkezik. [További információ](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ha szükséges, váltson át egy másik Microsoft 365-előfizetésre. [További információ](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ha az Office már telepítve van az RDS-kiszolgálón bármely más Microsoft 365-előfizetéssel, távolítsa el. Ha például a Vezérlőpultot fogja használni, \> távolítsa el a programot. Ha problémákat tapasztal, távolítsa el a [Microsoft támogatási és helyreállítási Segédet](https://aka.ms/SARA-OfficeUninstall-Alchemy) .

4. Az RDS-kiszolgálón bejelentkezés a Microsoft 365 felügyeleti központba a rendszergazdai fiókjával és a [microsoft 365-alkalmazások telepítése nagyvállalati](https://portal.office.com/OLS/MySoftware.aspx)verzióba.

5. Miután telepítette az Office-t, ***Ne nyisson meg vagy ne írjon be*** semmilyen Office-alkalmazást.

6. Az RDS-kiszolgálón engedélyezze a megosztott számítógép-aktiválást a beállításjegyzék szerkesztésével a következő lépésekkel:

1. Kattintson a jobb gombbal a Windows gombra a képernyő bal alsó sarkában, és válassza a Futtatás parancsot. A Megnyitás mezőbe írja be a **Regedit szót**, majd válassza az OK gombot.

2. Ha a rendszer kéri, válassza az Igen lehetőséget, ha az eszközén módosítani szeretné a beállításszerkesztőt.

3. A Rendszerleíróadatbázis-szerkesztőben adjon meg egy karakterláncot az **SharedComputerLicensing** , amelynek értéke 1 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Az RDS-kiszolgálón a ***Bejelentkezés végfelhasználóként*** , és [ellenőrizze, hogy engedélyezve van-e a Microsoft 365-alkalmazások nagyvállalatoknak való aktiválása a megosztott számítógépeken](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Ha további információra van kíváncsi a testreszabott példányokra vonatkozó előfeltételekről és útmutatásról az Office-telepítő eszközzel, olvassa el a [Microsoft 365-alkalmazások telepítése nagyvállalatoknak a távoli asztali szolgáltatások segítségével](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)című témakört.
  
A megosztott számítógép-aktiválással kapcsolatos hibák [elhárításáról a Microsoft 365-alkalmazások a nagyvállalati verzióhoz készült aktiválással kapcsolatos problémák elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)című témakörben talál további tájékoztatást.
  