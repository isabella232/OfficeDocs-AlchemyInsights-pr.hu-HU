---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676499"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Az 5.7.23-as hibakódú e-mailek kézbesítési problémáinak megoldása

Ellenőrizze a tartomány SPF DNS-rekordját egy nyilvánosan elérhető SPF- vagy DNS-rekordellenőrzőn az interneten.

Ellenőrizze, hogy a Microsoft nem azonosította-e a kimenő üzenetet levélszemétként, és nem jutott-e át a [magas kockázatú kézbesítési készleten.](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages) A magas kockázatú kézbesítési készletben lévő üzenetek nem felelnek meg az SPF-ellenőrzéseknek, ezért a célleveles szervezet nem fogadja el őket.

Ha a probléma továbbra is fennáll, előfordulhat, hogy kapcsolatba kell lépnie annak a levélszolgáltatónak az adminjával, amelyiknek e-mailt próbál küldeni. Jegyezze fel a részletes külső hibát a visszafordulási üzenetben. Előfordulhat, hogy a Microsoft támogatási szolgálata nem tud további segítséget nyújtani.
