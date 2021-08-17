---
title: Események hibaelhárítása e-mailből
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105354"
---
# <a name="troubleshooting-events-from-email"></a>Események hibaelhárítása e-mailből

1. Ellenőrizze, hogy engedélyezve van-e a szolgáltatás a postaládában: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Ezután nézze meg az "Events from Email" (E-mailből származó események) naplók **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Az "Események e-mailből" naplókban keresse meg a postaládában található elemnek megfelelő InternetMessageId-et.  

4. A TrustScore határozza meg, hogy az elemet hozzá szeretné-e adni vagy sem. Az események csak akkor lesznek hozzáadva, ha a TrustScore = "Megbízható".

A TrustScore tulajdonságot az üzenetfejlécben található SPF, Dkim vagy Dmarc tulajdonságok határozzák meg.

A tulajdonságok megtekintése:

**Asztali Outlook**

- Az elem megnyitása
- File -> Properties -> Internet Headers

vagy

**MFCMapi**

- Navigálás a Beérkezett üzenetek mappában
- Keresse meg a PR_TRANSPORT_MESSAGE_HEADERS_W

Ezeket a tulajdonságokat az adatokat az adatokat továbbítás és útválasztás során határozzák meg és rögzítik. További hibaelhárítási lépésként előfordulhat, hogy az SPF, a DKIM és.vagy a DMARC hiba elhárításáról a Transport Support ügyfélszolgálattal kell beszélnie.