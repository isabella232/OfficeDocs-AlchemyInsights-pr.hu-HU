---
title: Hiányzó e-mailek a karanténban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673716"
---
# <a name="missing-emails-in-quarantine"></a>Hiányzó e-mailek a karanténban "

A rendszergazdák [megtekinthetik, felszabadítják vagy törölhetik ezeket az üzeneteket.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Ha meg szeretné nyitni a biztonsági & megfelelőségi központot, lépjen a webhelyre [https://protection.office.com](https://protection.office.com/) . A karantén lap közvetlen megnyitásához lépjen a gombra [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

A Keresés az alábbi értékek alapján végezhető el:  

- **Üzenet azonosítója**: az üzenet globálisan egyedi azonosítója. Ha kijelöl egy üzenetet a listában, az  **üzenet azonosítójának**  értéke megjelenik a megjelenő  **részletek**  panelben. A rendszergazdák az [üzenet nyomon követésével](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) megkereshetik az üzeneteket és a hozzájuk tartozó üzenet-azonosító értékét.
- **Feladó e-mail-címe**: egyetlen feladó e-mail-címe.
- **Címzett e-mail-címe**: egyetlen címzett e-mail-címe.
- **Tárgy**: az üzenet teljes tárgyát használja. A keresés nem megkülönbözteti a kis-és nagybetűket.

Miután beírta a keresési feltételt, az ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** eredmény szűréséhez kattintson a frissítés gombra.  

A karanténba helyezett üzenetek és fájlok megtekintéséhez és kezelésére használt parancsmagok:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Exportálás – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- Előzetes verzió: ne feledje, hogy ez a parancsmag csak a SharePoint Online, a OneDrive vállalati verzió vagy a Teams ATP [-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)származó üzenetekre, nem pedig a malware-fájlokra vonatkozik.
- [Kiadás – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)