---
title: Biztonságosnak kell lennie egy tartománynak vagy egy e-mail-feladónak?
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803247"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Biztonságosnak kell lennie egy tartománynak vagy egy e-mail-feladónak?

- A **megbízható küldők listái nem ajánlottak** , mivel a szervezetet a levélszemét, az adathalász és a hamisítás elleni támadások megadásával nyitják meg.
- Ha azonban üzleti szükséglete van, azt **javasoljuk** , hogy e- **[mail-forgalom szabályait](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** használja ehhez a szolgáltatáshoz. Útmutatásunk szerint a küldő tartomány hitelesítése (a küldő tartomány ellenőrzése nem hamisítható meg). **Megjegyzés**: nem javasoljuk a téves pozitív adatok kezelését a megbízható küldők listáival, mert a levélszemét-szűrés alóli kivételek a szervezet biztonsági támadások számára való megnyitását szolgálják. Ha a felhasználó (k) tévesen levélszemétként vagy levélszemétként megjelölt üzeneteket fogad, kérjük, jelezze **[az üzeneteket és a fájlokat a Microsoftnak](https://protection.office.com/reportsubmission)**.
- **Elkerülhetők** a megbízható feladók az Outlookban, az engedélyezett feladók vagy a megengedett tartományok listája a levélszemét elleni szabályokban, mivel a feladók megkerülik az összes levélszemét-, svindli-és adathalász-védelmet, valamint a feladó hitelesítését (SPF, DKIM, DMARC). Ezt a módszert a legjobb csak ideiglenes teszteléshez használja.
