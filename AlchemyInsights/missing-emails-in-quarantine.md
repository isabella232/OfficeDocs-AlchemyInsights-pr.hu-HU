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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831736"
---
# <a name="missing-emails-in-quarantine"></a>Hiányzó e-mailek a karanténban"

A rendszergazdák [megtekinthetik, feladhatják vagy törölhetik ezeket az üzeneteket.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

A Biztonsági és & megnyitásához nyissa meg a következőt: [https://protection.office.com](https://protection.office.com/) . A karanténlap közvetlen megnyitásához nyissa meg a következőt: [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

A következő értékek alapján kereshet:  

- **Üzenetazonosító:** Az üzenet globálisan egyedi azonosítója. Ha kijelöl egy üzenetet a  listában, megjelenik  az Üzenetazonosító érték a megjelenő Részletek előgombra kattintva. A rendszergazdák az [üzenetkövetés](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) segítségével megkeresheti az üzeneteket és a hozzájuk tartozó üzenetazonosítókat.
- **Feladó e-mail-címe:** Egyetlen feladó e-mail-címe.
- **Címzett e-mail-címe:** Egyetlen címzett e-mail-címe.
- **Tárgy:** Használja az üzenet teljes tárgyát. A keresés nem megkülönbözteti a kis- és a nagybetűket.

Miután megadta a keresési feltételeket, a Frissítés gombra kattintva ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **szűrheti** a találatokat.  

A karanténban lévő üzenetek és fájlok megtekintéséhez és kezeléséhez a következő parancsmagok használhatók:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Ne feledje, hogy ez a parancsmag csak üzenetekhez használható, a SharePoint Online-hoz, a OneDrive Vállalati verzióhoz vagy a Teamshez nem tartalmaz kártevőfájlokat.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)