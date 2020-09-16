---
title: Események hibaelhárítása e-mailből
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658736"
---
# <a name="troubleshooting-events-from-email"></a>Események hibaelhárítása e-mailből

1. Ellenőrizze, hogy engedélyezve van-e a postaláda: **Get-EventsFromEmailConfiguration – <mailbox> identitás**

2. Ezután nézze meg az "események az e-mailből" naplók **exportálása – MailboxDiagnosticLogs <mailbox> – összetevő TimeProfile**

3. Az "események az e-mailből" naplókból keresse meg azt a InternetMessageId, amely megfelel a postaládában lévő elemnek.  

4. A TrustScore határozza meg, hogy az elem hozzáadódik-e vagy sem. Az események csak akkor kerülnek hozzáadásra, ha a TrustScore = "megbízható".

A TrustScore az SPF, a DKIM vagy a dMarc tulajdonság határozza meg, amely az üzenet fejlécében található.

A tulajdonságok megtekintése:

**Asztali Outlook**

- Az elem megnyitása
- Fájl-> tulajdonságok – > internetes fejlécek

vagy

**Mfcmapi felületet**

- Navigálás a Beérkezett üzenetek mappa elemei között
- Keresse meg a PR_TRANSPORT_MESSAGE_HEADERS_W

Ezeket a tulajdonságokat a szállítás és az Útválasztás során határozzák meg és rögzítik. További hibaelhárításért előfordulhat, hogy nyomon kell követnie az SPF, a DKIM vagy a DMARC hibáinak megfelelő átviteli támogatást.