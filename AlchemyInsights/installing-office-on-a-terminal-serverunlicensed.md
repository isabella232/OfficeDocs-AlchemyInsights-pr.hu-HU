---
title: Az Office telepítése Terminálkiszolgálóra – Nem licencelt
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
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322001"
---
# <a name="installing-office-on-a-terminal-server"></a>A Office telepítése terminálkiszolgálóra

Ha távoli asztali Windows (RDS) használatával, korábbi nevén Terminálszolgáltatások használatával Nagyvállalati Microsoft 365-alkalmazások központilag telepíteni egy Windows-kiszolgálón:
  
- Olyan előfizetéssel kell Microsoft 365, amely tartalmazza a Nagyvállalati Microsoft 365-alkalmazások, például Office 365 Nagyvállalati verzió E3 vagy Nagyvállalati E5 csomag. A Üzleti Microsoft 365-alkalmazások és a Üzleti Microsoft 365-alkalmazások Prémium csomagok nem tartalmazzák az Nagyvállalati Microsoft 365-alkalmazások.

- Engedélyeznie kell a [megosztott számítógép aktiválását.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Ha az alapértelmezett telepítési beállításokat Nagyvállalati Microsoft 365-alkalmazások alapértelmezett telepítési beállításokat használó Microsoft 365 Felügyeleti központ rdS-kiszolgálón szeretné telepíteni ***az*** adatokat, kövesse az alábbi lépéseket.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Ellenőrizze, Microsoft 365 milyen előfizetése van. [További információ](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ha szükséges, váltson másik előfizetésre, Microsoft 365 előfizetést. [További információ](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ha Office az RDS-kiszolgálóra már telepítve van a többi Microsoft 365 használatával, távolítsa el. Válassza például a Vezérlőpult Program \> eltávolítása parancsát. Távolítsa el a [Microsoft Támogatási és helyreállítási segéd](https://aka.ms/SARA-OfficeUninstall-Alchemy) használatával, ha problémákat okozhat.

4. Az RDS-kiszolgálón jelentkezzen be a Microsoft 365 Felügyeleti központ rendszergazdai fiókjával, és telepítse [a Nagyvállalati Microsoft 365-alkalmazások.](https://portal.office.com/OLS/MySoftware.aspx)

5. A Office után ne  nyisson meg és ne jelentkezzen be semmilyen Office alkalmazásba.

6. Az RDS-kiszolgálón engedélyezze a megosztott számítógép aktiválását a beállításjegyzék alábbi lépésekkel való szerkesztésével:

1. Kattintson a jobb gombbal Windows képernyő bal alsó sarkában lévő Windows gombra, és válassza a Futtatás lehetőséget. A Megnyitás mezőbe írja be a **regedit ,** parancsot, és válassza az OK gombot.

2. Válassza az Igen gombot, amikor a rendszer arra kéri, hogy engedélyezze a Beállításszerkesztőt az eszköz módosításához.

3. A Beállításszerkesztőben adjon meg egy 1-es értéket a **SharedComputerLicensing** karakterláncértékkel a HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration mappában.

7. Az RDS-kiszolgálón jelentkezzen be végfelhasználóként, és ellenőrizze, hogy ***engedélyezve*** van-e a megosztott számítógép [aktiválása Nagyvállalati Microsoft 365-alkalmazások.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Az előfeltételekről, a testre szabott telepítésekkel kapcsolatos, az Office-telepítő eszközzel kapcsolatos további információkért lásd: Nagyvállalati Microsoft 365-alkalmazások központi telepítés távoli asztali szolgáltatások [használatával.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
A megosztott számítógép aktiválásával kapcsolatos hibák elhárításáról A megosztott számítógép aktiválásával kapcsolatos hibák elhárítása a megosztott számítógép aktiválásával [Nagyvállalati Microsoft 365-alkalmazások.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  