---
title: Az Outlook asztali visszahívás vagy e-mail üzenet csere
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496113"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Visszahívni vagy kicserélni egy Outlook e-mail üzenet

- Mint a rendszergazda **Visszahívási üzenet PowerShell segítségével a felhasználók nevében**is. Az admin center üzenetek nem tudja visszahívni.
- **Csak a szervezet tagjai által küldött visszahívása üzeneteket**is. Ha az üzenet a Gmail címre lett küldve, például nem emlékszünk rá.
- Lehetőség van **csak a a PC-n Outlook 2016 küldött üzenetek visszahívása**. A felhasználó Outlook for Mac és a weben az Outlook üzenetet küld, ha nem tudja visszahívni.

A visszahívással vagy cserélje ki egy e-mail üzenetet:

1. A mappalistán az Outlook ablak a bal oldalon jelölje be az elküldött elemek mappába.
1. Kattintson duplán a nyissa meg a visszahívni kívánt üzenetet.
1. Kattintson az **üzenet** fülre, és válassza a **Műveletek** > **Az üzenet visszahívása**.
1. **Törli az üzenet olvasatlan példányait** , vagy **törli olvasatlan példányait és cserélje le egy új üzenetet**, és kattintson az **OK gombra**.
1. Ha csere üzenetet küldünk, írjuk meg az üzenetet, és válassza a **Küldés**.
1. A sikeres vagy sikertelen üzenet-visszahívásról függ, hogy a címzett az Outlook beállításait. A visszahívás ellenőrzése, olvassa el [a](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)lépéseket.

Keresse meg, és a szervezet e-mail üzenetek törlése

- Ha Ön nem egy globális felügyeleti, a fiók az elektronikus adatok feltárása kezelője szerepkör vagy üzenetek kereséséhez való keresés szerepkör hozzá kell adni. Üzenetek törlése, szüksége lesz a Szervezetkezelés szerepkör vagy a Keresés és a kiürítés szerepkör csatlakozni. Ezek a szerepkörök az engedélyeket a [biztonsági és kompatibilitási központ](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Keresés a tartalom létrehozása](https://docs.microsoft.com/office365/securitycompliance/content-search) az üzenet törlése.
- [Biztonsági és Megfelelési központba PowerShell kapcsolódni](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Többtényezős hitelesítést használ, lásd a [Csatlakozás az Office 365 biztonsági és kompatibilitási központ PowerShell többtényezős hitelesítést használ](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).