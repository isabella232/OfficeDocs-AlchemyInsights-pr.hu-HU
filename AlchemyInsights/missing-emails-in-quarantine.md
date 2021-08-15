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
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026224"
---
# <a name="missing-emails-in-quarantine"></a>Hiányzó e-mailek a karanténban"

A rendszergazdák [megtekinthetik, feladhatják vagy törölhetik ezeket az üzeneteket.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

A Biztonsági és & megnyitásához nyissa meg a következőt: [https://protection.office.com](https://protection.office.com/) . A karanténlap közvetlen megnyitásához nyissa meg a következőt: [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

A következő értékek alapján kereshet:  

- **Üzenetazonosító:** Az üzenet globálisan egyedi azonosítója. Ha kijelöl egy üzenetet a  listában, megjelenik  az Üzenetazonosító érték a megjelenő Részletek előgombra kattintva. A rendszergazdák az [üzenetkövetés](/microsoft-365/security/office-365-security/message-trace-scc) segítségével megkeresheti az üzeneteket és a hozzájuk tartozó üzenetazonosítókat.
- **Feladó e-mail-címe:** Egyetlen feladó e-mail-címe.
- **Címzett e-mail-címe:** Egyetlen címzett e-mail-címe.
- **Tárgy:** Használja az üzenet teljes tárgyát. A keresés nem megkülönbözteti a kis- és a nagybetűket.

Miután megadta a keresési feltételeket, a Frissítés gombra kattintva ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **szűrheti** a találatokat.

A karanténban lévő üzenetek és fájlok megtekintéséhez és kezeléséhez a következő parancsmagok használhatók:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Ne feledje, hogy ez a parancsmag csak az üzenetekhez érhető el, a Microsoft Defendertől származó kártevőfájlok nem az Office 365 SharePoint Online- vagy SharePoint-, OneDrive Vállalati verzió- vagy Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)