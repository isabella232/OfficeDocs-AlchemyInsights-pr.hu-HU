---
title: Antispam-5.7.23 hibakódú
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717327"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Az e-mailek kézbesítésével kapcsolatos problémák megoldása a hibakódok 5.7.23 hibakódú

Ellenőrizze a tartomány SPF DNS-rekordját a nyilvánosan elérhető SPF-vagy DNS-rekordok ellenőrzésekor a weben.

Ellenőrizze, hogy a kimenő üzenet a Microsofttól kapott-e levélszemétként, és a [nagy kockázatú kézbesítési készleten](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)keresztül továbbítódik-e. A magas kockázatú kézbesítési készlet üzenetei nem jutnak el az SPF-ellenőrzésekhez, ezért a cél e-mail-szervezet nem fogadja el őket.

Ha a probléma nem szűnik meg, előfordulhat, hogy fel kell vennie a figyelmét annak a levelezési állomásnak a rendszergazdájára, amelyhez e-mailt próbál küldeni. Jegyezze fel a visszafordulási üzenetben elérhető részletes külső hibát. Előfordulhat, hogy a Microsoft ügyfélszolgálata nem tud további segítséget nyújtani.
