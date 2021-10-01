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
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041008"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Az Nagyvállalati Microsoft 365-alkalmazások telepítése megosztott használatra RDS- vagy Terminálkiszolgálón, illetve VDI-n

A távoli Microsoft 365-alkalmazások (RDS), korábbi terminálszolgáltatások használatával való telepítéséhez a következőt kell használnia:

- Az egyszerű javítás használatával alapértelmezés szerint engedélyezheti a TLS 1.2-t, ha az Windows régebbi verzióját használja (például Windows 7 SP1, Windows Server 2008 R2). Az egyszerű javításról és további információról a Frissítés a [TLS 1.1 és A TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)alapértelmezett biztonságos protokollként való engedélyezéséhez a Windows winhttps://Windows. 
- Olyan csomagja van, amely tartalmazza a Nagyvállalati Microsoft 365-alkalmazások (korábban Office 365 Plust). Ilyen például a Office 365 E3 csomag vagy Microsoft 365 E5, illetve az Project vagy az Visio asztali verzióját (például Project 3. csomag vagy Visio 2. csomag) tartalmazó csomag, illetve az Microsoft 365 Vállalati prémium verzió csomag, amely tartalmazza a Üzleti Microsoft 365-alkalmazások.
- Engedélyezze a megosztott számítógép aktiválását. További információt A megosztott számítógép [aktiválásának áttekintése](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)az Microsoft 365-alkalmazások.

**Megjegyzés:** Ha megosztott Microsoft 365-alkalmazások módban telepíteni, töltse le és futtassa a [Microsoft Támogatási és helyreállítási segéd.](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds) Az előfeltételekről, a telepítési utasításokról és a telepítésnek az Office-telepítő eszközzel történő testreszabására vonatkozó útmutatásért lásd: Microsoft 365-alkalmazások központi telepítés távoli asztali [szolgáltatásokkal.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

A megosztott számítógép aktiválásával kapcsolatos hibák megoldásához lásd:

- [A megosztott számítógép aktiválásával kapcsolatos problémák elhárítása Microsoft 365-alkalmazások](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Microsoft 365-appok visszaállítása nagyvállalati aktiválási állapotba](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Ha rdS-Microsoft 365-alkalmazások szeretné telepíteni az alapértelmezett telepítési Microsoft 365 Felügyeleti központ, kövesse az alábbi lépéseket:

1. Ellenőrizze, Microsoft 365 milyen csomagja van. További információ: [Milyen előfizetéssel rendelkezik?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Ha szükséges, váltson egy másik Microsoft 365 csomagra. További információ: Frissítés másik [csomagra.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Ha Microsoft 365-alkalmazások telepítette az RDS-kiszolgálóra más nem kompatibilis csomagokkal, távolítsa el a **Vezérlőpult** Program eltávolítása  >  **parancsával.** Ha problémákat okozhat, távolítsa el a [Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy)Támogatási és helyreállítási segéd.

1. Az RDS-kiszolgálón jelentkezzen be a Microsoft 365 Felügyeleti központ rendszergazdai fiókjával, és telepítse [a Office.](https://portal.office.com/OLS/MySoftware.aspx)

   A Office után ne nyisson meg és ne jelentkezzen be semmilyen Office alkalmazásba.

1. Az RDS-kiszolgálón engedélyezze a megosztott számítógép aktiválását a beállításjegyzék szerkesztésével:

   1. Kattintson a jobb gombbal Windows képernyő bal alsó sarkában lévő Windows gombra, és válassza a **Futtatás lehetőséget.** A Megnyitás mezőbe írja be a **regedit** parancsot, majd kattintson az **OK** gombra.

   1. Amikor a rendszer arra kéri, hogy engedélyezze a Beállításszerkesztőnek az eszközén való módosításokat, válassza az **Igen gombot.**

   1. A Beállításszerkesztőben a HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration részen adjon meg egy 1-es értéket a **SharedComputerLicensing** **karakterláncértékkel.**

1. Az RDS-kiszolgálón jelentkezzen be végfelhasználóként, és ellenőrizze, hogy engedélyezve van-e a megosztott számítógép aktiválása Microsoft 365-alkalmazások. 

   Részletekért lásd: Annak ellenőrzése, hogy engedélyezve van-e a megosztott számítógép [aktiválása Microsoft 365-alkalmazások.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)