---
title: Az Outlook asztali visszahívása vagy lecserélése az e-mail üzenetre
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496113"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook e-mail üzenet visszahívása vagy lecserélése

- Mint az admin, akkor **felidézni üzeneteket nevében a felhasználók segítségével PowerShell**. Nem lehet visszahívni az üzeneteket az Admin Center.
- Csak a **szervezetben lévő személyeknek elküldött üzeneteket lehet visszahívni**. Ha például az üzenetet Gmail-címre küldték, nem lehet visszahívni.
- **Csak az Outlook 2016-ből küldött üzenetek visszahívhatók a számítógépen**. Ha a felhasználó az Outlook for Mac vagy az Outlook alkalmazással küld üzenetet a weben, akkor nem tudja felidézni.

E-mail üzenet felidézése vagy cseréje:

1. Az Outlook ablakának bal oldalán található mappalistán jelölje ki az elküldött elemek mappát.
1. Kattintson duplán a visszahívni kívánt üzenetre.
1. Válassza az **üzenet** fület, majd válassza a **műveletek** > **visszahívása ezt az üzenetet**.
1. Jelölje be az **üzenet olvasatlan másolatainak törlése** vagy az **olvasatlan másolatok törlése és a lecserélés egy új üzenetre**választógombot, majd kattintson **az OK gombra**.
1. Ha cserecikk üzenetet küldünk, írjuk be az üzenetet, majd nyomjuk meg a **küld**választógombot.
1. Az üzenet-visszahívás sikere vagy sikertelenje a címzettek Outlook programban megadott beállításaitól függ. A visszahívás ellenőrzéséhez szükséges lépések a [jelen cikkben](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)találhatók.

E-mail üzenetek keresése és törlése a szervezeten belül

- Ha Ön nem egy globális rendszergazda, akkor fiókját hozzá kell adni az eDiscovery Manager szerepkörhöz vagy a megfelelőségi keresés felügyeleti szerepkörhöz az üzenetek kereséséhez. Az üzenetek törléséhez csatlakoznunk kell a Szervezetkezelés szerepkörcsoporthoz vagy a keresés és tisztítás felügyeleti szerepkörhöz. Az ezekhez a szerepkörökhöz tartozó engedélyeket a [biztonsági és megfelelőségi központ](https://go.microsoft.com/fwlink/?linkid=2083731)rendeli hozzá.
- [Hozzon létre egy tartalomkeresést](https://docs.microsoft.com/office365/securitycompliance/content-search) a törlendő üzenet megkereséséhez.
- [Összeköt-hoz biztonság és engedékenység központ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Többtényezős hitelesítés használata esetén tekintse meg [a Kapcsolódás az Office 365 biztonsági és megfelelőségi központ PowerShell környezethez a többtényezős hitelesítés használatával](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)című témakört.