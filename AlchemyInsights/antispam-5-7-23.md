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
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932171"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Az 5.7.23-as hibakódos levélk kézbesítési problémáinak megoldása

Ellenőrizze tartománya SPF DNS-rekordját egy nyilvánosan elérhető SPF vagy DNS-rekord-ellenőrző segítségével az interneten.

Győződjön meg arról, hogy a kimenő üzenetet nem azonosította levélszemétként a Microsoft, és az üzenetet a Magas kockázatú kézbesítési [készleten keresztül kézbesíti.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) A Magas kockázatú kézbesítési készletbe küldött üzenetek nem fognak átesni az SPF-ellenőrzéseken, ezért a cél levelezési szervezet nem fogadja el őket.

Ha a probléma nem szűnik meg, előfordulhat, hogy kapcsolatba kell lépnie annak a levelezési szolgáltatónak a rendszergazdával, amelybe e-mailt próbál küldeni. Jegyezze fel a visszapattanó üzenetben elérhető részletes külső hibát. Előfordulhat, hogy a Microsoft ügyfélszolgálata nem tud további segítséget nyújtani.
