---
title: Értesítések a Yammerben
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
- "9002878"
- "5480"
ms.openlocfilehash: 8e7c03f2b557a7d3c409b2ee418df055d0569ee6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833581"
---
# <a name="notifications-in-yammer"></a>Értesítések a Yammerben

Annak érdekében, hogy értesítést kapjon a releváns beszélgetésekben történő új tevékenységről, [a Yammer ](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)e-mailen, illetve (ha Ön mobileszközön használja a Yammert) leküldéses értesítéseken keresztül küld értesítést. A Yammer alapértelmezés szerint több tevékenységtípus esetén küld értesítéseket a hálózatában. A felhasználók a Yammer-webhelyen keresztül frissíthetik az e-mail-beállításaikat, a leküldéses értesítések pedig a mobilalkalmazáson keresztül konfigurálhatók. 

A Yammer bevezette az [interaktív e-mailek támogatását az Outlookban](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Bizonyos e-mailek (az üzenet másolata) interaktívvá válnak a webes Outlookban. Egy jövőbeli frissítés ezt az Outlook más verziói számára is elhozza.

**Értesítéstípusok a Yammerben**

- E-mailek (Egy csoport frissítései, valaki meghívja Önt egy csoportba, üzenetet kap a Beérkezett üzenetek mappájában stb.)
- Leküldéses értesítések (A mobileszközökre küldve, ha megemlítik Önt, üzenetek fogadása a Beérkezett üzenetek mappában stb.)
- Asztali előugró ablakok (Ha telepítve van a Yammer asztali alkalmazás, akkor megjeleníti a felhasználók által „bejelentési“ értesítésnek nevezett értesítéseket.)
- Csengő értesítések (A Yammer webhelyén belül a felhasználók a különböző eseményekre vonatkozó értesítéseket fognak látni. Előfordulhat, hogy ezekhez az értesítésekhez nem mindig tartozik társított e-mail vagy leküldéses értesítés.)

Elérhetők további [részletes információk az értesítésekről](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Értesítések kezelése**

Saját értesítéseiket a felhasználóknak kell kezelniük. Elérhetők információk a [Yammer e-mailes és mobil értesítéseinek engedélyezéséről és letiltásáról](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

A rendszergazdák a felhasználók nevében nem tudják letiltani az összes értesítést, illetve szabályozni az értesítéseket. A rendszergazdák [szabályozhatják az e-mailekben található emblémát, valamint azt, hogy a felhasználóknak meg kell-e erősíteniük az üzeneteket](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer), amelyeket e-mailben küldtek.

**A szervezet számos felhasználója számára küldött e-mail értesítések**

Időnként előfordul, hogy a Yammer egyetlen e-mail értesítést küld, amelyet a vártnál sokkal több felhasználó megkap a szervezetben. Ez akkor történik, ha egy terjesztési lista vagy más, nem egyéni típusú e-mail-cím van a Yammerhez hozzáadva. A Yammer nem tudja minden esetben, hogy egy e-mail-cím egyetlen felhasználóhoz tartozik-e, vagy egy olyan e-mail-cím, amellyel egy e-mailt sok címzett számára kézbesítenek. A probléma előfordulása esetén lépéseket kell tennie ahhoz, hogy [felfüggessze (inaktiválja) az érvénytelen felhasználót az e-mail-címmel](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) a Yammeren. 

Annak érdekében, hogy csökkentse a probléma előfordulásának esélyét, a következőket kell tennie:

1. [Az Office 365-identitás érvényesítése](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) a Yammerben.
2. A külső feladók esetén a szervezet számára történő e-mail-küldés letiltása, illetve a feladók korlátozása egy jóváhagyott listára.

A probléma előfordulása esetén:

1. Azonosítsa az e-mail címzettjét, amelynek egyeznie kell a Yammer-felhasználóval. Például az all-in-sales@fabrikam.com egy DL az összes értékesítő számára. Ez a DL azonosítható a felhasználók által fogadott Yammer-e-mailek közül.
2. A [Hálózatfelügyeleten belül az inaktiválás (felfüggesztés) funkció](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) használata az all-in-sales@fabrikam.com e-mail-címmel rendelkező felhasználó felfüggesztésére. A felfüggesztés visszavonható, így biztonságosabb a törlésnél. A felhasználó törlése 90 nap elteltével automatikusan megtörténik.
3. Tetszés szerint áttekintheti a [Felhasználó exportálását](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers), hogy azonosítsa azokat a nem felhasználói e-mail-címeket, amelyeket fel kell függeszteni.
