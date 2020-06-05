---
title: Események el- és nagy-amerikai hibáinak elhárítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569140"
---
# <a name="troubleshooting-events-from-email"></a>Események el- és nagy-amerikai hibáinak elhárítása

1. Ellenőrizze, hogy a szolgáltatás engedélyezve van-e a postaládához: **Get-EventsFromEmailConfiguration -Identity <mailbox> **

2. Ezután nézd meg a "Események e-mailből" naplók **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Az "Események e-mailből" naplókban keresse meg a postaládában lévő elemnek megfelelő InternetMessageId azonosítót.  

4. A TrustScore határozza meg, hogy az elemet hozzáadják-e vagy sem. Az események csak akkor kerülnek hozzáadásra, ha a TrustScore = "Megbízható".

A TrustScore-t az Üzenetfejlécben található SPF, Dkim vagy Dmarc tulajdonságok határozzák meg.

A következő tulajdonságok megtekintése:

**Asztali Outlook**

- Az elem megnyitása
- Fájl -> tulajdonságai -> internetes fejlécek

vagy

**MFCMapi**

- Keresse meg a beérkezett üzenetek mappában lévő elemet
- Keresse meg a PR_TRANSPORT_MESSAGE_HEADERS_W

Ezeket a tulajdonságokat a szállítás és az útválasztás során határozzák meg és rögzítik. További hibaelhárítás, előfordulhat, hogy nyomon kell követnie a Transport Support kapcsolatos hibák SPF, DKIM és.vagy DMARC.