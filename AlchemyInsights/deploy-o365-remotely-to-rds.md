---
title: A Microsoft 365-alkalmazások központi telepítése az RDS, a terminálkiszolgáló vagy a VDI rendszeren megosztott használatra
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 22ded616e82b2e82023b55a1d3ca6251cfb71712
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745537"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>A Microsoft 365-alkalmazások központi telepítése az RDS, a terminálkiszolgáló vagy a VDI rendszeren megosztott használatra

A Microsoft 365-alkalmazások központi telepítése a nagyvállalati verzió (RDS) szolgáltatással, korábbi nevén Terminálszolgáltatások:
- Rendelkeznie kell egy olyan Microsoft 365 vállalati verziós csomaggal vagy Office 365-csomaggal, amely tartalmazza a nagyvállalati Microsoft 365-alkalmazásokat, például az Office 365 nagyvállalati E3 vagy a nagyvállalati E5 csomagot.
   > [!NOTE] 
   > A Microsoft 365-alkalmazások vállalati verzió és a Microsoft 365 Business Premium standard csomag nem tartalmazza a Microsoft 365-alkalmazásokat a nagyvállalatoknak.
- Engedélyeznie kell a [megosztott számítógép aktiválását](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Azt is megteheti, hogy letölti és futtatja a [Microsoft támogatási és helyreállítási Segédet](https://aka.ms/SaRA_OfficeSCA_M365Portal) a Microsoft 365-alkalmazások nagyvállalatoknak való telepítéséhez a megosztott számítógép-aktiválási módban.

Ha többet szeretne tudni a testreszabott példányokra vonatkozó előfeltételekről, útmutatásról és útmutatásról az Office-telepítő eszközzel, olvassa el a [Microsoft 365-alkalmazások telepítése nagyvállalatoknak a távoli asztali szolgáltatások segítségével](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)című témakört.

A megosztott számítógép aktiválásával kapcsolatos hibák elhárítása:
- Lásd: a [Microsoft 365-alkalmazások nagyvállalati verzióhoz készült megosztott számítógép-aktiválással kapcsolatos problémák elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Lásd: [Microsoft 365-appok visszaállítása nagyvállalati aktiválási állapotba](https://go.microsoft.com/fwlink/?linkid=2109218).

Ha a Microsoft 365-alkalmazásokat a nagyvállalati verzióra szeretné telepíteni a Microsoft 365 felügyeleti központból, ***amely az alapértelmezett telepítési beállításokat használja***, kövesse az alábbi lépéseket:

1.    Ellenőrizze, hogy milyen előfizetéssel rendelkezik. [További információ](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Ha szükséges, váltson át egy másik előfizetésre. [További információ](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Ha az Office már telepítve van az RDS-kiszolgálón bármely más Microsoft-előfizetéssel, távolítsa el. Ha például a **Vezérlőpultot**fogja használni,  >  **távolítsa el a programot**. Ha problémákat tapasztal, távolítsa el a [Microsoft támogatási és helyreállítási Segédet](https://aka.ms/SARA-OfficeUninstall-Alchemy) .
4.    Az RDS-kiszolgálón bejelentkezés a Microsoft 365 felügyeleti központba a rendszergazdai fiókjával és a [microsoft 365-alkalmazások telepítése nagyvállalati](https://portal.office.com/OLS/MySoftware.aspx)verzióba.
5.    Miután telepítette az Office-t, ***Ne nyisson meg vagy ne írjon be*** semmilyen Office-alkalmazást.
6.    Az RDS-kiszolgálón engedélyezze a megosztott számítógép-aktiválást a beállításjegyzék szerkesztésével a következő lépésekkel:
   1. Kattintson a jobb gombbal a Windows gombra a képernyő bal alsó sarkában, és válassza a **Futtatás**parancsot. A Megnyitás mezőbe írja be a **Regedit szót**, majd válassza az **OK**gombot.
   2. Ha a rendszer kéri, válassza az **Igen** lehetőséget, ha az eszközén módosítani szeretné a beállításszerkesztőt.
   3. A Rendszerleíróadatbázis-szerkesztőben adjon meg egy karakterláncot az **SharedComputerLicensing** , amelynek értéke 1 HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Az RDS-kiszolgálón a ***Bejelentkezés végfelhasználóként*** , és [ellenőrizze, hogy engedélyezve van-e a Microsoft 365-alkalmazások nagyvállalatoknak való aktiválása a megosztott számítógépeken](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

