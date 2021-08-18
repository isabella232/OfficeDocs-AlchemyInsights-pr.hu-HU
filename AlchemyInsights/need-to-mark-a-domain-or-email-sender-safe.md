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
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319950"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Meg kell jelölnie egy tartomány vagy e-mail feladóját?

- A megbízható **feladók** listájának használata nem ajánlott, mivel a szervezetet levélszemét, adatszemét és hamisítási támadások ellen nyitja meg.
- Ha azonban van üzleti követelmény, azt javasoljuk, hogy **ehhez** Flow **[levelezési](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** szabályokat. Útmutatásunk biztosítja a feladók hitelesítését (ellenőrzi, hogy a küldő tartományt nem hamisják-e meg). 
    **Megjegyzés:** Nem javasoljuk a vak pozitív üzenetek biztonságos feladók listákkal való kezelésének alkalmazását, mert a levélszemétszűrés alóli kivételek megnyitják szervezetét a biztonsági támadások ellen. Ha a felhasználó(k) helytelenül levélszemétként vagy levélszemétként megjelölt üzeneteket kapnak, jelentse az üzeneteket és fájlokat a **[Microsoftnak.](https://protection.office.com/reportsubmission)**
- Széf Az Outlook, az Engedélyezett feladók vagy a levélszemét-szűrési házirendek engedélyezett tartománylistáiban található feladók kerülendők, mert a feladók megkerülik az összes levélszemét- és hamisítás-védelmi és adatvédelmet, valamint a feladók hitelesítését (SPF, DKIM, DMARC).  Ez a módszer csak ideiglenes teszteléshez ajánlott.
- Az X-Forefront-Antispam-Report (X-Forefront-Antispam-Report) üzenetfejléc (SFV:SFE, SFV:SKA, SFV:SKN) ellenőrzésével lehet ellenőrizni, hogy az adott **[e-mail át van-e](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** kerülve a Levélszemét elleni védelemre.
- Mivel a Microsoft alapértelmezés szerint meg szeretné tartani ügyfeleink [biztonságát,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)a bérlői webhelyek bizonyos felülbírálásai nem alkalmazhatók a kártevőkre és a nagy megbízhatóságú adathalászatra. Ezek a felülbírálások a következők: o Engedélyezett feladók listája vagy engedélyezett tartománylisták (levélszemét-szűrési házirendek) o Outlook Széf feladók o IP Allow List (kapcsolatszűrés) 
- Az egyetlen felülbírálás, amely lehetővé teszi a nagy megbízhatóságú adathalász üzeneteknek a szűrés megkerülését, az Exchange szabályok (más néven átviteli szabályok) alkalmazása. Ha a szűrés megkerülése e-mail-forgalom szabályaival is meg kell kerülnie, tekintse meg a Levélszemét-megbízhatósági szint (SCL) beállítása az üzenetekben e-mail-forgalom **[szabályaival (SCL).](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**