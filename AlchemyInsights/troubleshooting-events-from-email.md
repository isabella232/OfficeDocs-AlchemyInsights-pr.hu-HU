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
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834841"
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