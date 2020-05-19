---
title: Meg kell jelölnie egy tartomány- vagy e-mail feladói széfet?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281150"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Meg kell jelölnie egy tartomány- vagy e-mail feladói széfet?

- A **biztonságos feladói listák** használata nem ajánlott, mivel megnyitja a szervezetet a levélszemét, a phish és a hamisítás igéző támadásai számára.
- Ha azonban üzleti követelmény van, **javasoljuk, hogy** ehhez használja a **[Mail Flow-szabályokat.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Útmutatónk biztosítja a küldő hitelesítését (ellenőrzi, hogy a küldő tartomány nem kerül hamisításra). **Megjegyzés:** Nem javasoljuk a hamis pozitív adatok biztonságos feladói listák használatával történő kezelését, mivel a levélszemétszűrés alóli kivételek megnyithatják a szervezetet a biztonsági támadások előtt. Ha a felhasználó(k) olyan üzeneteket kapnak, amelyek helytelenül spamként vagy levélszemétként vannak megjelölve, kérjük, **[jelentsék az üzeneteket és fájlokat a Microsoftnak.](https://protection.office.com/reportsubmission)**
- **Kerülni kell** a megbízható feladókat az Outlook ban, az Engedélyezett feladók listáját vagy a levélszemét-ellenes házirendekben engedélyezett tartománylistát, mivel a feladók megkerülik az összes levélszemét-, hamisítás- és adathalászat-védelmet, valamint a feladó hitelesítését (SPF, DKIM, DMARC). Ez a módszer csak ideiglenes tesztelésre használható.
