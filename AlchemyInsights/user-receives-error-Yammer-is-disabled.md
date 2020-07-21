---
title: 'A felhasználó hibaüzenetet kap: AADSTS7000112 Yammer le van tiltva'
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198057"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>A felhasználó hibaüzenetet kap: AADSTS7000112 Yammer le van tiltva

Ha az "AADSTS7000112: Application '000000005-0000-0ff1-000000000000000"(Yammer) le van tiltva" hibaüzenet jelenik meg, probléma van az Azure AD szolgáltatásfőelemével. Előfordulhat, hogy egy rendszergazda letiltotta az egyszerű szolgáltatást a Yammerhez való hozzáférés letiltásához.

A szolgáltatásnév letiltása nem ajánlott, és további problémákat okozhat. A Yammer felhasználói hozzáférésének letiltására vonatkozó támogatott módszerről a [Yammer-hozzáférés kikapcsolása a Microsoft 365-felhasználók számára](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)című témakörben talál további információt.  

A probléma kijavítása az Azure Portalon, és a Yammer felhasználói hozzáférésének visszaállítása:

1.  Nyissa meg az Azure Active Directory lapot, és válassza **a Vállalati alkalmazások** **csoportban a bal** oldali navigációs ablakban.
3.  Írja be az **Office 365 Yammer kifejezést** a keresőmezőbe, és válassza ki az alkalmazás nevét a beállítások megnyitásához.
4.  A bal oldali navigációs ablakban válassza a **Tulajdonságok** lehetőséget a **Kezelés** csoportban.
5.  Állítsa be a felhasználók számára engedélyezve a **bejelentkezéshez jelölőnégyzetet,** majd válassza **a** **Mentés**lehetőséget.
6.  Jelentkezzen be ismét a Yammerbe. Előfordulhat, hogy törölnie kell a cookie-kat.

Másik lehetőségként futtassa a PowerShell-parancsokat az érték beállításához. További információt a ["Sajnáljuk, de nem sikerül bejelentkeznünk" hibaüzenet jelenik meg, amikor az Office 365 Yammer csempéjére kattint.](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365) 