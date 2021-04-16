---
title: Meg kell jelölnie egy tartomány vagy e-mail feladóját?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792134"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Meg kell jelölnie egy tartomány vagy e-mail feladóját?

- A megbízható **feladók** listájának használata nem ajánlott, mivel a szervezetet levélszemét, adatszemét és hamisítási támadások ellen nyitja meg.
- Ha azonban van üzleti követelmény, azt javasoljuk, **hogy** ehhez az **[e-mail-forgalomra](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** vonatkozó szabályokat használja. Útmutatásunk biztosítja a feladók hitelesítését (ellenőrzi, hogy a küldő tartományt nem hamis használják-e fel). **Megjegyzés:** Nem javasoljuk a vak pozitív üzenetek biztonságos feladók listákkal való kezelésének alkalmazását, mert a levélszemétszűrés alóli kivételek megnyitják szervezetét a biztonsági támadások ellen. Ha a felhasználó(k) helytelenül levélszemétként vagy levélszemétként megjelölt üzeneteket kapnak, kérjük, jelentse az üzeneteket és fájlokat a **[Microsoftnak.](https://protection.office.com/reportsubmission)**
- Az Outlook megbízható feladói, az engedélyezett feladók listája  és az engedélyezett tartománylista a levélszemét-szűrési házirendek során kerülendő, mert a feladók megkerülik az összes levélszemét, hamisítás és adatvédelmet, valamint a feladók hitelesítését (SPF, DKIM, DMARC). Ez a módszer csak ideiglenes teszteléshez ajánlott.
