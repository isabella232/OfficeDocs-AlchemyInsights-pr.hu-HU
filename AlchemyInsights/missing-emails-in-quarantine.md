---
title: Hiányzó e-mailek karanténban
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329664"
---
# <a name="missing-emails-in-quarantine"></a>Hiányzó e-mailek karanténban

A rendszergazdák [megtekinthetik, feladhatják és törölhetik ezeket az üzeneteket](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

A (Microsoft 365 Defender) portálon a <https://security.microsoft.com> Karantén **áttekintése** \> **hoz tovább.** Vagy közvetlenül a Karantén lapra **való ugráshoz** használja a következőt: <https://security.microsoft.com/quarantine> .  

A használható keresési/szűrőértékekkel kapcsolatos további információkért lásd: Karanténba helyezett üzenetek és fájlok kezelése rendszergazdaként az [EOP szolgáltatásban.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

A karanténban lévő üzenetek és fájlok megtekintéséhez és kezeléséhez használt parancsmagok a következőek:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Ne feledje, hogy ez a parancsmag csak üzenetekhez érhető el, a SharePoint-, OneDrive- vagy Széf-mellékletből származó Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
