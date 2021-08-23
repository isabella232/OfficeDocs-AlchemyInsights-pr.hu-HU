---
title: Egy tévesen pozitív levélszemétről szeretne bejelentést küldeni a Microsoftnak?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396617"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Levélszemétnek minősített szabályos üzenetei vannak?

Bosszantó lehet, amikor egy valódi e-mail a Levélszemét mappába vagy a karanténba kerül. Vegye figyelembe az alábbi hamis pozitív állítások leggyakoribb okait:

**Bérlői felülbírálások (leggyakoribb)** Ez teljes mértékben az Ön ható maga alatt van, hogy szervizbe tetsszen.

Küldje el az üzenetet Microsoft 365 Defender az érintett házirendek és szabályok elemzéséhez; néhány perc alatt elérhetők az adatok.
Tekintse át vagy módosítsa a házirendeket vagy szabályokat az adott esetben. 

**Végfelhasználói felülbírálások (közös)** Ez teljes mértékben az Ön ható maga alatt van, hogy szervizbe tetsszen. 

Küldje el az üzenetet Microsoft 365 Defender az érintett házirendek és szabályok elemzéséhez; néhány perc alatt elérhetők az adatok. 

Ha egy üzenet azért lett blokkolva, mert egy felhasználó Letiltott feladók listájában található címről küldte el, a fejlécek között szerepel a levélszemétszűrés "SFV:BLK" értesítés.

**A feladók e-mail-hitelesítése** Ez részlegesen a saját vezérlőn belül található a szerviz szervizhez.

Küldje el az üzenetet, hogy elemezze a feladó e-mail-hitelesítésének sikertelen voltát a kézbesítéskor; találatok egy napon belül elérhetők. 

Ha Öné a küldési infrastruktúra, ellenőrizze, hogy miként igazítja azt az SPF, DKIM és DMARC protokollhoz, és győződjön meg arról, hogy a cél levelezőrendszerek megbízik a tartományról küldött üzenetekben. Másik lehetőségként lépjen kapcsolatba a feladóval a DNS-konfigurációjuk megcímzésével.

**A Microsoft szűrési döntését** Ez részlegesen a saját vezérlőn belül található a szerviz szervizhez.

Küldje el az üzenetet, és jelentse az üzenetet biztonságosként; rescan results are available within a day. Akkor használja a bérlői engedélyezése/letiltása listát, ha ön nem ért egyet bizonyos helyzetekben a szűrési döntésekkel. Nem szabad azonban végleg megkerülni a Microsoft szűrési döntését. 

További információ:

- Engedélyezze a végfelhasználóknak, hogy üzeneteket küldjenek a Microsoftnak. A Microsoft ezeket a beküldött adatokat a levelezésvédelmi technológiák hatékonyságának javítására használja, és a beküldött jelentésekben is megjelennek, hogy Ön a házirendek frissítésére utaló jelzésként használja őket. 

- Az üzenetek elemzésre való beküldését bemutató rövid videót az Üzenetek küldése [elemzésre.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Levélszemétgyanús, phish, URL-címek és fájlok küldése a Microsoftnak rendszergazdai beküldés használatával](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [A bérlői fiók allow/block listájának kezelése](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Levélszemét-szűrési fejlécek a Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Kimenő levélszemét elleni védelem az EOP-ban](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)