---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821413"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Az 5.7.23-as hibakódos levélk kézbesítési problémáinak megoldása

Ellenőrizze tartománya SPF DNS-rekordját egy nyilvánosan elérhető SPF vagy DNS-rekord-ellenőrző segítségével az interneten.

Győződjön meg arról, hogy a kimenő üzenetet nem azonosította levélszemétként a Microsoft, és az üzenetet a Magas kockázatú kézbesítési [készleten keresztül kézbesíti.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) A Magas kockázatú kézbesítési készletbe küldött üzenetek nem fognak átesni az SPF-ellenőrzéseken, ezért a cél levelezési szervezet nem fogadja el őket.

Ha a probléma nem szűnik meg, előfordulhat, hogy kapcsolatba kell lépnie annak a levelezési szolgáltatónak a rendszergazdával, amelybe e-mailt próbál küldeni. Jegyezze fel a visszapattanó üzenetben elérhető részletes külső hibát. Előfordulhat, hogy a Microsoft ügyfélszolgálata nem tud további segítséget nyújtani.
