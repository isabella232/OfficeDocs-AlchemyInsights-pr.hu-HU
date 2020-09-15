---
title: Az Outlook asztali e-mail-üzenet visszahívása vagy cseréje
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663992"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook-üzenet visszahívása vagy cseréje

- Rendszergazdaként a **PowerShell segítségével visszahívhatja az üzeneteket a felhasználók nevében**. A felügyeleti központból nem lehet visszahívni az üzeneteket.
- **Csak a szervezet tagjainak küldött üzeneteket lehet visszahívni**. Ha az üzenetet Gmail-címre küldték, például nem tudja visszahívni.
- **A számítógépen csak az Outlook 2016-ból küldött üzeneteket lehet visszahívni**. Ha egy felhasználó a Mac Outlookban vagy a webes Outlookban küld üzenetet, nem lehet visszahívni.

E-mailek visszahívása vagy cseréje:

1. Az Outlook ablakának bal oldalán található mappa ablaktáblában válassza az elküldött elemek mappát.
1. Kattintson duplán a felidézni kívánt üzenetre a megnyitásához.
1. Válassza az **üzenet** fület, majd a **műveletek**  >  **visszahívása az üzenettel**lehetőséget.
1. Válassza az **üzenet olvasatlan példányainak törlése** vagy az **olvasatlan példányok törlése, majd a csere egy új üzenettel**lehetőséget, és kattintson **az OK gombra**.
1. Ha helyettesítő üzenetet küld, írja meg az üzenetet, és válassza a **Küldés**gombot.
1. Az üzenet visszahívásának sikere vagy kudarca az Outlook címzett beállításaitól függ. A visszahívás ellenőrzésének lépései a következő [cikkben](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)olvashatók.

E-mail-üzenetek keresése és törlése a szervezetben

- Ha nem globális rendszergazda, a fiókját fel kell vennie az eDiscovery-kezelő szerepkörbe vagy a megfelelőségi keresési felügyeleti szerepkörbe az üzenetek kereséséhez. Üzenetek törléséhez csatlakoznia kell a szervezeti vagy a keresési és törlési felügyeleti szerepkörhöz. Ezek a szerepkörök engedélyei a [biztonsági és megfelelőségi központban](https://go.microsoft.com/fwlink/?linkid=2083731)lesznek kiosztva.
- A törlendő üzenet megtalálásához [hozzon létre egy keresési tartalmat](https://docs.microsoft.com/microsoft-365/compliance/content-search) .
- [Csatlakozás a biztonsági és megfelelőségi központ powershellhez](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Többtényezős hitelesítés esetén a [Csatlakozás a Microsoft 365 biztonsági és megfelelőségi központ powershellhez többtényezős hitelesítéssel](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)című témakörben tájékozódhat.