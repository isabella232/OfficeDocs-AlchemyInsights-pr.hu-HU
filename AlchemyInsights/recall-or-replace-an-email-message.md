---
title: E-mail-üzenet visszahívása vagy cseréje
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353508"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>E-mail-üzenet visszahívása vagy cseréje a Microsoft 365

- **Csak a szervezet tagjainak küldött üzeneteket lehet visszahívni**. Ha például az üzenetet Gmail-címre küldte, a program nem tudja visszahívni.
- **Csak a PC-ről küldött üzeneteket lehet visszahívni**. Ha egy felhasználó a Mac Outlookban vagy a webes Outlookban küld üzenetet, nem lehet visszahívni.
- Bérlői rendszergazdaként a **PowerShell használatával visszahívhatja az üzeneteket a felhasználók nevében** (további információt az [e-mailek keresése és törlése](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)című témakörben talál).
- A felügyeleti központból nem lehet visszahívni az üzeneteket. További információt az "e-mail-üzenetek keresése és törlése a szervezetben" című témakörben olvashat.

**Elküldött e-mailek visszahívása vagy cseréje**

1. Az Outlook ablakának bal oldalán található mappa ablaktáblában válassza az elküldött elemek mappát.
2. Nyissa meg a visszahívni kívánt üzenetet. Az üzenet megnyitásához duplán kell kattintania. Ha kijelöli az üzenetet, hogy az olvasóablakban jelenjen meg, ne engedélyezze az üzenet visszahívását.
3. Az üzenet lapon válassza a **műveletek**  >  **visszahívása ezt az üzenetet** lehetőséget.
4. Válassza az **üzenet olvasatlan példányainak törlése** vagy az **olvasatlan példányok törlése, majd a csere egy új üzenettel** lehetőséget, és válassza **az OK gombot**.
5. Ha helyettesítő üzenetet küld, írja meg az üzenetet, és válassza a **Küldés** gombot.
6. Az üzenet visszahívásának sikere vagy kudarca az Outlook címzettek beállításaitól függ.

Ha további információra van szüksége a visszahívás ellenőrzéséről, olvassa el az [elküldött e-mailek visszahívása vagy cseréje](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)című témakört.

Ha meg **_szeretné keresni és törölni szeretné a szervezetében lévő e-maileket_**, akkor a legegyszerűbb, ha Ön globális rendszergazda. Ha nem globális rendszergazda, fiókját fel kell vennie az eDiscovery-kezelő szerepkörcsoport szerepkör-csoportjához vagy a megfelelőségi keresési szerepkörbe. Üzenetek törléséhez csatlakoznia kell a szervezeti vagy a keresési és törlési felügyeleti szerepkörhöz. Az e szerepkörökhöz tartozó engedélyeket a [biztonsági & megfelelőségi központban](https://protection.office.com/)lehet kiosztani.

1. A törlendő üzenet megtalálásához [hozzon létre egy keresési tartalmat](https://docs.microsoft.com/microsoft-365/compliance/content-search) .
2. [Csatlakozás a biztonsági & megfelelőségi központ powershellhez](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Ha MFA-t (többtényezős hitelesítést) használ, olvassa el [a csatlakozás a Microsoft 365 biztonsági & megfelelőségi központ PowerShell a többtényezős hitelesítéssel](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)című témakört.
