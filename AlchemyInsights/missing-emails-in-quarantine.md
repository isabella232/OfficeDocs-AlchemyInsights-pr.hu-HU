---
title: Hiányzó e-mailek a karanténban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569231"
---
# <a name="missing-emails-in-quarantine"></a>Hiányzó e-mailek a karanténban"

A rendszergazdák [megtekinthetik, feladhatják vagy törölhetik ezeket az üzeneteket.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

A Biztonsági & megfelelőségi központ megnyitásához nyissa meg a [https://protection.office.com](https://protection.office.com/) t. A Karantén lap közvetlen megnyitásához nyissa meg a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) at.  

A következő értékek szerint kereshet:  

- **Üzenetazonosító**: Az üzenet globálisan egyedi azonosítója. Ha kijelöl egy üzenetet a listában, az **Üzenetazonosító** értéke megjelenik a **megjelenő Részletek** úszó panelen. A rendszergazdák [az üzenetek nyomon követésével](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) kereshetik meg az üzeneteket és a hozzájuk tartozó Üzenetazonosító-értékeket.
- **Feladó e-mail címe**: Egyetlen feladó e-mail címe.
- **Címzett e-mail címe**: Egyetlen címzett e-mail címe.
- **Tárgy**: Az üzenet teljes témáját használhatja. A keresés nem a kis- és nagybetűket nem érzékeny.

Miután megadta a keresési feltételeket, kattintson a ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Frissítés gombra,** a Frissítés gombra az eredmények szűréséhez.  

A karanténban lévő üzenetek és fájlok megtekintéséhez és kezeléséhez használt parancsmagok a következők:
- [Törlés-KaranténÜzenet](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Vegye figyelembe, hogy ez a parancsmag csak üzenetekhez készült, a SharePoint Online, a OneDrive Vállalati verzió vagy a Teams ATP-ből származó kártevőfájlokhoz nem.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)