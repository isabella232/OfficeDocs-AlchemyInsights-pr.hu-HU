---
title: Az Nagyvállalati Microsoft 365-alkalmazások telepítése megosztott használatra RDS- vagy Terminálkiszolgálón, illetve VDI-n
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325605"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Az Nagyvállalati Microsoft 365-alkalmazások telepítése megosztott használatra RDS- vagy Terminálkiszolgálón, illetve VDI-n

Az Nagyvállalati Microsoft 365-alkalmazások távoli asztali szolgáltatások (RDS) használatával, korábbi nevén Terminálszolgáltatások használatával:

- Vállalati verziós csomagra Microsoft 365 vagy egy Office 365 csomagra van Nagyvállalati Microsoft 365-alkalmazások, például Office 365 Nagyvállalati verzió E3 vagy Nagyvállalati E5 csomag.
   **Megjegyzés:** A Üzleti Microsoft 365-alkalmazások és Microsoft 365 Vállalati standard verzió csomagok nem tartalmaznak Nagyvállalati Microsoft 365-alkalmazások.
- Engedélyeznie kell [a megosztott számítógép aktiválását.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

**Megjegyzés:** A Microsoft-webhelyet letöltheti és futtathatja is, [Támogatási és helyreállítási segéd](https://aka.ms/SaRA_OfficeSCA_M365Portal) megosztott Nagyvállalati Microsoft 365-alkalmazások módban telepítheti az kódot.

Az előfeltételekről, a telepítési utasításokról és a testre szabott telepítésekkel kapcsolatos, az Office-telepítő eszközzel kapcsolatos további információkért lásd: Nagyvállalati Microsoft 365-alkalmazások központi telepítés távoli asztali [szolgáltatásokkal.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

A megosztott számítógép aktiválásával kapcsolatos hibák kijavítása:

- Lásd: A megosztott számítógép aktiválásával kapcsolatos problémák [elhárítása Nagyvállalati Microsoft 365-alkalmazások.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- Lásd: [Microsoft 365-appok visszaállítása nagyvállalati aktiválási állapotba](https://go.microsoft.com/fwlink/?linkid=2109218).

Ha az alapértelmezett telepítési beállításokat Nagyvállalati Microsoft 365-alkalmazások alapértelmezett telepítési beállításokat használó Microsoft 365 Felügyeleti központ rdS-kiszolgálón szeretné telepíteni ***az*** adatokat, kövesse az alábbi lépéseket:

1. Ellenőrizze, hogy milyen előfizetése van. [További információ](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Ha szükséges, váltson egy másik előfizetésre. [További információ](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Ha Office microsoft-előfizetéssel már telepítve van az RDS-kiszolgálóra, távolítsa el. Válassza például a **Vezérlőpult Program**  >  **eltávolítása parancsát.** Távolítsa el a [Microsoft Támogatási és helyreállítási segéd](https://aka.ms/SARA-OfficeUninstall-Alchemy) használatával, ha problémákat okozhat.
4. Az RDS-kiszolgálón jelentkezzen be a Microsoft 365 Felügyeleti központ rendszergazdai fiókjával, és telepítse [a Nagyvállalati Microsoft 365-alkalmazások.](https://portal.office.com/OLS/MySoftware.aspx)
5. A Office után ne  nyisson meg és ne jelentkezzen be semmilyen Office alkalmazásba.
6. Az RDS-kiszolgálón engedélyezze a megosztott számítógép aktiválását a beállításjegyzék alábbi lépésekkel való szerkesztésével:
   1. Kattintson a jobb gombbal Windows képernyő bal alsó sarkában lévő Windows gombra, és válassza a **Futtatás lehetőséget.** A Megnyitás mezőbe írja be a **regedit** parancsot, majd kattintson az **OK** gombra.
   2. Válassza **az Igen gombot,** amikor a rendszer arra kéri, hogy engedélyezze a Beállításszerkesztőt az eszköz módosításához.
   3. A Beállításszerkesztőben adjon meg egy 1-es értéket a **SharedComputerLicensing** karakterláncértékkel a HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration mappában.
   4. Az RDS-kiszolgálón jelentkezzen be végfelhasználóként, és ellenőrizze, hogy ***engedélyezve*** van-e a megosztott számítógép [aktiválása Nagyvállalati Microsoft 365-alkalmazások.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
