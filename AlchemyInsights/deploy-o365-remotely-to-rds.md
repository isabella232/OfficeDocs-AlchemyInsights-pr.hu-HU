---
title: Microsoft 365-alkalmazások központi telepítése nagyvállalati használatra RDS- vagy Terminálkiszolgálón, illetve VDI-n keresztül
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200675"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365-alkalmazások központi telepítése nagyvállalati használatra RDS- vagy Terminálkiszolgálón, illetve VDI-n keresztül

A Microsoft 365-alkalmazások telepítése nagyvállalati környezetben a Távoli asztali szolgáltatások (RDS), korábbi nevén Terminálszolgáltatások használatával:

- A csomagnak olyan Microsoft 365 Vállalati verziós csomagra vagy Office 365-csomagra van lennie, amely tartalmazza a nagyvállalati Microsoft 365-alkalmazásokat, például az Office 365 Nagyvállalati E3 vagy Nagyvállalati E5 csomagokat.
   > [!NOTE]
   > A Vállalati Microsoft 365-alkalmazások és a Microsoft 365 Vállalati standard verziós csomagok nem tartalmazzák a nagyvállalati Microsoft 365-appokat.
- Engedélyeznie kell [a megosztott számítógép aktiválását.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> A [Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) Támogatási és helyreállítási segédet letöltve és futtatva is telepítheti a nagyvállalati Microsoft 365-appokat megosztott számítógép-aktiválási módban.

Az előfeltételekről, a telepítési utasításokról és a testre szabott telepítésekkel kapcsolatos, az Office-telepítő eszközzel kapcsolatos útmutatásért lásd: [Microsoft 365-alkalmazások](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)központi telepítése nagyvállalati használatra távoli asztali szolgáltatásokkal.

A megosztott számítógép aktiválásával kapcsolatos hibák kijavítása:

- Lásd: [A nagyvállalati Microsoft 365-alkalmazások](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)megosztott számítógép aktiválásával kapcsolatos hibák elhárítása.
- Lásd: [Microsoft 365-appok visszaállítása nagyvállalati aktiválási állapotba](https://go.microsoft.com/fwlink/?linkid=2109218).

Ha az alapértelmezett telepítési beállításokat használó Microsoft 365 Felügyeleti központ rdS szolgáltatáson keresztüli nagyvállalati Microsoft 365-alkalmazásait szeretné ***telepíteni,*** kövesse az alábbi lépéseket:

1. Ellenőrizze, hogy milyen előfizetése van. [További információ](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Ha szükséges, váltson egy másik előfizetésre. [További információ](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Ha az Office már telepítve van az RDS-kiszolgálón más Microsoft-előfizetésekkel, távolítsa el. Válassza például a **Vezérlőpult Program**  >  **eltávolítása parancsát.** Távolítsa el a [Microsoft Támogatási és helyreállítási](https://aka.ms/SARA-OfficeUninstall-Alchemy) segéddel, ha problémákat okozhat.
4. Az RDS-kiszolgálón jelentkezzen be a Microsoft 365 Felügyeleti központba rendszergazdai fiókjával, és telepítse a [Nagyvállalati Microsoft 365-alkalmazások alkalmazást.](https://portal.office.com/OLS/MySoftware.aspx)
5. Az Office telepítése után ***ne*** nyisson meg semmilyen Office-alkalmazást, és ne jelentkezzen be.
6. Az RDS-kiszolgálón engedélyezze a megosztott számítógép aktiválását a beállításjegyzék alábbi lépésekkel való szerkesztésével:
   1. Kattintson a jobb gombbal a Windows gombra a képernyő bal alsó sarkában, és válassza a **Futtatás lehetőséget.** A Megnyitás mezőbe írja be a **regedit** parancsot, majd kattintson az **OK** gombra.
   2. Válassza **az Igen gombot,** amikor a rendszer arra kéri, hogy engedélyezze a Beállításszerkesztőt az eszköz módosításához.
   3. A Beállításszerkesztőben adja meg a **SharedComputerLicensing** karakterláncértéket 1-es értékkel az HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration mappában.
   4. Az RDS-kiszolgálón  jelentkezzen be végfelhasználóként, és ellenőrizze, hogy a megosztott számítógép aktiválása engedélyezve van-e a [Nagyvállalati Microsoft 365-alkalmazásokhoz.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
