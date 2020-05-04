---
title: Microsoft 365-ös alkalmazások telepítése vállalati használatra távoli asztali szolgáltatások, terminálkiszolgáló vagy VDI-n
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 51512b29f8d37ce6c39ece5bb704cb01e88e463d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010256"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365-ös alkalmazások telepítése vállalati használatra távoli asztali szolgáltatások, terminálkiszolgáló vagy VDI-n

Microsoft 365-alkalmazások központi telepítése nagyvállalatoknak a Távoli asztali szolgáltatások (RDS) korábbi nevén Terminálszolgáltatások használatával:
- Rendelkeznie kell egy Microsoft 365 Vállalati verziós csomaggal vagy egy Olyan Office 365-csomaggal, amely tartalmazza a nagyvállalati Microsoft 365 alkalmazásokat, például az Office 365 Nagyvállalati E3 vagy a Nagyvállalati E5 csomagot.
   > [!NOTE] 
   > A Microsoft 365 vállalati alkalmazások és a Microsoft 365 Vállalati prémium standard szintű csomagok nem tartalmazzák a nagyvállalati Microsoft 365 alkalmazásokat.
- Engedélyeznie kell a [megosztott számítógép aktiválását.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> A [Microsoft támogatási és helyreállítási segédjét](https://aka.ms/SaRA_OfficeSCA_M365Portal) is letöltheti és futtathatja a Microsoft 365 vállalati alkalmazások megosztott számítógép-aktiválási módban történő telepítéséhez.

Az Office-telepítő eszköz használatával a testreszabott telepítésekkel kapcsolatos előfeltételekről, telepítési utasításokról és útmutatásról a [Microsoft 365-alkalmazások telepítése nagyvállalatoknak a Távoli asztali szolgáltatások használatával](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)című témakörben talál további információt.

A megosztott számítógép-aktiválással kapcsolatos hibák kijavítása:
- Lásd: [Problémák a Microsoft 365 vállalati verzióinak megosztott számítógép-aktiválásával kapcsolatos problémák elhárítása című témakörben.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Lásd: [Microsoft 365-appok visszaállítása nagyvállalati aktiválási állapotba](https://go.microsoft.com/fwlink/?linkid=2109218).

Ha a Microsoft 365 vállalati alkalmazásokat az RDS szolgáltatásba szeretné telepíteni a Microsoft 365 Felügyeleti központból, ***amely az alapértelmezett telepítési beállításokat használja,*** kövesse az alábbi lépéseket:

1.    Ellenőrizze, hogy milyen előfizetéssel rendelkezik. [További információ](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Ha szükséges, váltson másik előfizetésre. [További információ](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Ha az Office már telepítve van az RDS-kiszolgálón bármely más Microsoft-előfizetéssel, távolítsa el azt. Például a **Vezérlőpult eltávolítása** > **Uninstall a program**elemre. Eltávolítás a [Microsoft támogatási és helyreállítási segédsegítségével,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ha problémákba ütközik.
4.    Az RDS-kiszolgálón jelentkezzen be a Microsoft 365 felügyeleti központba a rendszergazdai fiókkal, és [telepítse a Microsoft 365 vállalati alkalmazásokat.](https://portal.office.com/OLS/MySoftware.aspx)
5.    Az Office telepítése után ***ne nyisson meg és ne jelentkezzen be*** egyetlen Office-alkalmazásba sem.
6.    Az RDS-kiszolgálón engedélyezze a megosztott számítógép aktiválását a rendszerleíró adatbázis szerkesztésével az alábbi lépésekkel:
   1. Kattintson a jobb gombbal a képernyő bal alsó sarkában lévő Windows gombra, és válassza a **Futtatás parancsot.** A Megnyitás mezőbe írja be a **regedit parancsot,** majd kattintson **az OK gombra.**
   2. Válassza az **Igen** lehetőséget, amikor a rendszer kéri, hogy a Rendszerleíróadatbázis-szerkesztő módosíthassa az eszközt.
   3. A Beállításjegyzék-szerkesztőben adjon meg egy **SharedComputerLicensing** karakterlánc-értéket 1-es értékkel a HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration csoportban.
   4. Az RDS-kiszolgálón ***jelentkezzen be végfelhasználóként,*** és [ellenőrizze, hogy a microsoft 365-ös vállalati alkalmazások esetében engedélyezve van-e a megosztott számítógép aktiválása.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

