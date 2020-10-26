---
title: Előfizetés/fiók letiltva szabály
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003559"
- "6676"
ms.openlocfilehash: 6a350c6bca18306e64f647cfa3a7f14fa204109b
ms.sourcegitcommit: 9626d39e5891f83774ba31574a00b0bae92ad442
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/24/2020
ms.locfileid: "48758586"
---
# <a name="azure-subscription-disabled"></a>Azure-előfizetés letiltva

Az Azure-előfizetése le tud tiltani, mert lejárt a hitelkerete, elérte a kiadási korlátot, lejárt számlával rendelkezik, megtalálta a hitelkártyája korlátját, vagy azért, mert a fiók rendszergazdája megszakította az előfizetést. Az előfizetés ismételt engedélyezésének módjáról alább tájékozódhat. További információ: az [Azure-előfizetés újraaktiválása](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support)

**Az Azure-előfizetés ismételt engedélyezése (az előfizetés véletlenül lemondva)** A [fiók rendszergazdája](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) újraaktiválhatja a lemondott fizetési mód előfizetését a fiók központjában:

1. Bejelentkezés a [fiók központba](https://account.windowsazure.com/Subscriptions)
2. Jelölje ki a lemondott előfizetést. Kattintson az **újraaktiválás** gombra.

Egyéb előfizetési típusok esetén [forduljon az ügyfélszolgálathoz](https://portal.azure.com/?#blade/Microsoft_Azure_Support/HelpAndSupportBlade) , és kérje újra az előfizetést.

**Lejárt hitelkártya**

Amikor feliratkozik az **Azure ingyenes fiókjára** , ingyenes próbaverziós előfizetést kap, amely az Azure-kreditek 30 napig és 12 hónapig ingyenes szolgáltatást nyújt az $200. 30 nap elteltével az Azure letiltotta az előfizetést. Az előfizetése le van tiltva, hogy védve legyen az előfizetéséhez tartozó hitelkártyán és ingyenes szolgáltatáson kívüli használati díjakról. Az Azure Services használatának folytatásához [frissítenie kell az előfizetést](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support). A frissítés után az előfizetése még 12 hónapig is elérhető az ingyenes szolgáltatásokhoz. Csak a szabad szolgáltatásokon és mennyiségeken kívüli felhasználásra kell fizetnie.  
További információ: [lejárt hitelkártya](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support#your-credit-is-expired)

**Kiadási korlát elérve**

Ha a használat eléri a kiadási korlátot, az Azure letiltja az előfizetést a számlázási időszak hátralévő részében. Az előfizetése le van tiltva, hogy védve legyen az előfizetéséhez tartozó hitelen kívüli használati díjak véletlen használatából. Ha el szeretné távolítani a kiadási korlátot, olvassa el az [Azure kiadások korlátozása](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)című témakört.  
További információ: [a kiadások korlátjának elérése](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled?WT.mc_id=Portal-Microsoft_Azure_Support#you-reached-your-spending-limit)

**Lejárt számlázás**

A korábbi esedékes egyenleg feloldásáról az [Azure-előfizetés múltbeli esedékes egyenlegének feloldása az Azure-hoz küldött e-mailek esetén](https://docs.microsoft.com/azure/billing/billing-azure-subscription-past-due-balance?WT.mc_id=Portal-Microsoft_Azure_Support)című témakörben talál további tájékoztatást.

**A számla túllépi a hitelkártyás korlátot**

A probléma megoldásához [váltson másik hitelkártyára](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support). Vagy ha vállalkozást képvisel, [számlás fizetésre válthat](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice?WT.mc_id=Portal-Microsoft_Azure_Support).

**Megjegyzés** : a program új előfizetési évforduló (SA) dátumot rendel az újból felhasználható előfizetésekhez. Annak a napoknak (intervallumnak) a száma, amelyben az előfizetést felfüggesztették, a program hozzáadja az eredeti biztonsági társítási dátumhoz. A 29, 30 vagy 31 hónapra eső évfordulós idő a következő hónap első napjának értéke lesz.  
Például

- Az eredeti előfizetési évfordulója a 25;
- Az előfizetést felfüggesztették az 10/3-ben, és újból engedélyezte a 10/9-on;
- Az előfizetést 6 napra letiltották (6-os intervallum);
- Az intervallum megjelenik az eredeti biztonsági társításban, és az összeg az új biztonsági társítás dátuma lesz (25 + 6 = 31). 

**Megjegyzés** : ebben a példában az, hogy az SA dátuma most már 28-nál nagyobb, az új SA dátuma a következő hónap első száma lesz.

**Ajánlott dokumentumok**

- [Előfizetés váltása](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [Előfizetés lemondása](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace/?source=datamarket)
- A [fiók-rendszergazda](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) megkeresése
- [Mi a teendő, ha az Azure-előfizetés le lesz tiltva?](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure kiadási korlát](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)
