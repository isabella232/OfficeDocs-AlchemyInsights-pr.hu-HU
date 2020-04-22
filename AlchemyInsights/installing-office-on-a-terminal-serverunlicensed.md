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
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763219"
---
# <a name="installing-office-on-a-terminal-server"></a>Az Office telepítése terminálkiszolgálóra

Microsoft 365-alkalmazások vállalati telepítéséhez Windows Server en a Távoli asztali szolgáltatások (RDS) használatával, amelyet korábbi nevén Terminálszolgáltatások nak neveztek el:
  
- Olyan Microsoft 365-előfizetéssel kell rendelkeznie, amely tartalmazza a nagyvállalati Microsoft 365 alkalmazásokat, például az Office 365 Nagyvállalati E3 vagy nagyvállalati E5 verziót. A Microsoft 365 vállalati alkalmazások és a Microsoft 365 Apps for Business Premium csomagok nem tartalmazzák a nagyvállalati Microsoft 365 alkalmazásokat.

- Engedélyeznie kell a [megosztott számítógép aktiválását.](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)

Ha a Microsoft 365 vállalati alkalmazásokat az RDS szolgáltatásba szeretné telepíteni a Microsoft 365 Felügyeleti központból, ***amely az alapértelmezett telepítési beállításokat használja,*** kövesse az alábbi lépéseket.

> [!TIP]
> A [Microsoft támogatási és helyreállítási segédjét](https://aka.ms/SaRA_OfficeSCA_M365Portal) is letöltheti és futtathatja a Microsoft 365 vállalati alkalmazások megosztott számítógép-aktiválási módban történő telepítéséhez.
  
1. Ellenőrizze, hogy milyen Microsoft 365-előfizetéssel rendelkezik. [Ismerje meg, hogyan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Szükség esetén váltson másik Microsoft 365-előfizetésre. [Ismerje meg, hogyan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Ha az Office már telepítve van az RDS-kiszolgálón bármely más Microsoft 365-előfizetéssel, távolítsa el azt. Például a Vezérlőpult \> eltávolítása parancsra. Eltávolítás a [Microsoft támogatási és helyreállítási segédsegítségével,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ha problémákba ütközik.

4. Az RDS-kiszolgálón jelentkezzen be a Microsoft 365 felügyeleti központba a rendszergazdai fiókkal, és [telepítse a Microsoft 365 vállalati alkalmazásokat.](https://portal.office.com/OLS/MySoftware.aspx)

5. Az Office telepítése után ***ne nyisson meg és ne jelentkezzen be*** egyetlen Office-alkalmazásba sem.

6. Az RDS-kiszolgálón engedélyezze a megosztott számítógép aktiválását a rendszerleíró adatbázis szerkesztésével az alábbi lépésekkel:

1. Kattintson a jobb gombbal a képernyő bal alsó sarkában lévő Windows gombra, és válassza a Futtatás parancsot. A Megnyitás mezőbe írja be a **regedit parancsot,** majd kattintson az OK gombra.

2. Válassza az Igen lehetőséget, amikor a rendszer kéri, hogy a Rendszerleíróadatbázis-szerkesztő módosíthassa az eszközt.

3. A Beállításjegyzék-szerkesztőben adjon meg egy **SharedComputerLicensing** karakterlánc-értéket 1-es értékkel a HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration csoportban.

7. Az RDS-kiszolgálón ***jelentkezzen be végfelhasználóként,*** és [ellenőrizze, hogy a microsoft 365-ös vállalati alkalmazások esetében engedélyezve van-e a megosztott számítógép aktiválása.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)

Az előfeltételekről, a telepítési utasításokról és a testreszabott telepítésekkel kapcsolatos útmutatásról az Office központi telepítési eszközével a [Microsoft 365-alkalmazások telepítése nagyvállalatoknak a Távoli asztali szolgáltatások használatával](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)című témakörben talál további információt.
  
A megosztott számítógép-aktiválással kapcsolatos hibák kijavításáról olvassa el A [Microsoft 365 vállalati alkalmazások megosztott számítógép-aktiválásával kapcsolatos problémák elhárítása című témakört.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)
  