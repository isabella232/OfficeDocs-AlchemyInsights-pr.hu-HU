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
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286682"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Meg kell jelölnie egy tartomány vagy e-mail feladóját?

- A megbízható **feladók** listájának használata nem ajánlott, mivel a szervezetet levélszemét, adatszemét és hamisítási támadások ellen nyitja meg.
- Ha azonban van üzleti követelmény, azt javasoljuk, hogy **ehhez** Flow **[levelezési szabályokat.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Útmutatásunk biztosítja a feladók hitelesítését (ellenőrzi, hogy a küldő tartományt nem hamis használják-e fel). **Megjegyzés:** Nem javasoljuk a vak pozitív üzenetek biztonságos feladók listákkal való kezelésének alkalmazását, mert a levélszemétszűrés alóli kivételek megnyitják szervezetét a biztonsági támadások ellen. Ha a felhasználó(k) helytelenül levélszemétként vagy levélszemétként megjelölt üzeneteket kapnak, kérjük, jelentse az üzeneteket és fájlokat a **[Microsoftnak.](https://protection.office.com/reportsubmission)**
- Széf A Outlook, az Engedélyezett feladók vagy a levélszemét-szűrési házirendek engedélyezett tartománylistáiban található feladók kerülendők, mert a feladók megkerülik az összes levélszemét, hamisítás és adatvédelmet, valamint a feladók hitelesítését (SPF, DKIM, DMARC).  Ez a módszer csak ideiglenes teszteléshez ajánlott.
- Az X-Forefront-Antispam-Report (X-Forefront-Antispam-Report) üzenetfejléc (SFV:SFE, SFV:SKA, SFV:SKN) ellenőrzésével lehet ellenőrizni, hogy az adott **[e-mail át van-e](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** kerülve a Levélszemét elleni védelemre.
- Mivel a Microsoft alapértelmezés szerint meg szeretné tartani ügyfeleink [biztonságát,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)a bérlői webhelyek bizonyos felülbírálásai nem alkalmazhatók a kártevőkre és a nagy megbízhatóságú adathalászatra. Ezek a felülbírálások a következők lehetnek: o Engedélyezett feladók listája vagy engedélyezett tartománylisták (levélszemét-szűrési házirendek) o Outlook Széf ip allow list (kapcsolatszűrés) 
- Az egyetlen felülbírálás, amely lehetővé teszi a nagy megbízhatóságú adathalász üzeneteknek a szűrés megkerülését, az Exchange szabályok (más néven átviteli szabályok) alkalmazása. Ha az e-mail-forgalomra vonatkozó szabályok használatával meg kell kerülnie a szűrést, további információ: Levélszemét-megbízhatósági szint beállítása e-mail-forgalom szabályaival az **[üzenetekben.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**