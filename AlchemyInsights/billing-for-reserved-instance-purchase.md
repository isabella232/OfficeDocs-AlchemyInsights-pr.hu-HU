---
title: Fenntartott példány vásárlásának számlázása
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
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820324"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fenntartott példány vásárlásának számlázása

A lefoglalt példány megvásárlását a vásárláskor kiválasztott előfizetéshez kötött fizetési módra terheljük. Az előfizetés típusának nagyvállalati szerződésnek (ajánlatszámnak: MS-AZR-0017P), "Fizetés mint Ön által" (ajánlatszám: MS-AZR-0003P), Microsoft ügyfélszerződésnek vagy CSP-nek kell lennie.

- Nagyvállalati előfizetés esetén a díjakat levonjuk a regisztráció pénzügyi kötelezettségvállalási egyenlegéből, vagy a díjakat túlóraként terheljuk meg.
- A "Fizetés mint You Go" előfizetés esetén a díjakat hitelkártyás vagy számlás fizetési módra számlázjuk az előfizetésben.

**Foglalás lemondása**

- **Önkiszolgáló szolgáltatás:** Saját maga is lemondhatja vagy kicserélheti a fenntartott példányokat az [Azure Portal használatával.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Jelölje ki a foglalást, és kattintson a visszatérítésre vagy a csere elemre. Felhívjuk a figyelmét arra, hogy tulajdonosi hozzáféréssel kell rendelkezik a foglalási rendeléshez a csere vagy visszatérítés érdekében. Kizárólag a Foglaláshoz való hozzáférés esetén nem jogosult visszatérítésre vagy cserére. Kérje meg a foglalási rendelés tulajdonosát, hogy adjon Önnek hozzáférést a foglalási rendeléshez.
- **Exchange-házirend:** Más, azonos típusú foglalások lefoglalását is át lehet cserélni – a foglalási csere nem tartalmazza **a** szobafoglalási összeget. Az új foglalással kapcsolatos teljes kötelezettségvállalásnak nagyobbnak kell lennie, mint az átváltott foglalások visszatérítési összege és a jövőbeli havi kifizetések összege (ha van ilyen).
- **Visszatérítési szabályzat:** A visszatérítés összege és a lemondott jövőbeli kifizetések nem haladhatja meg az 50 000 usd-t egy 12 hónapos görgető ablakban. Jelenleg nem **számolunk fel** pénzvisszatérítési díjat, de a jövőbeli visszatérítések után rá lehet fizetni.

**Kivételek:** Az önkiszolgáló csere- és lemondási funkció nem érhető el az Egyesült Egyesült Állam kormányzati nagyvállalati szerződésének ügyfelei számára

- **Az API/PS/CLI** támogatása nem érhető el lemondáshoz és visszatérítéshez Önkiszolgáló tőzsdére és visszatérítésre [Azure-foglalások esetén](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Az önkiszolgáló csere- és lemondási funkció nem érhető el az Egyesült Államok kormányzati nagyvállalati szerződésének ügyfelei számára. Más, egyesült egyesült államokkal kapcsolatos előfizetési típusok, például a "Fizetés mint Ön-go" és a "CSP" támogatottak

További információ: [A visszaküldési](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) és a cseretranzakciók feldolgozása További információ: [Exchange-](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) és visszatérítési szabályzatok További [kérdések: Fenntartott példányok dokumentumok](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) megtekintése

**Meglévő fenntartott példány cseréje (Önkiszolgáló)**

Ugyanezen típusú más foglalások foglalását is kicserélheti. Ha már nincs rá szüksége, visszatéríthet egy 50 000 USD összeget is évente. Az önkiszolgáló csere- és lemondási funkció nem érhető el az Egyesült Államok kormányzati nagyvállalati szerződésének ügyfelei számára. Az Egyesült Államok kormányzati előfizetési típusai, például a "Pay-As-You-Go" és a "CSP" előfizetések támogatottak. A meglévő foglalások cseréjéhez vagy visszatérítésére tulajdonosi hozzáféréssel kell lennie a foglalási rendelésben.

Az alábbi lépések végigvezetik a tranzakció befejezésének eljárásán.

1.Jelentkezzen be az [Azure Portalba.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Jelölje ki a visszatérítendő foglalásokat, és kattintson az **Exchange** 2 gombra.Válassza ki a megvásárolni kívánt VM-terméket, és írja be a mennyiséget. Győződjön meg arról, hogy az új beszerzési összeg nagyobb, mint a vissza visszaút összege Határozza meg a megfelelő méretet [a vásárlás előtt.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.A tranzakció áttekintése és befejezése

**Visszatérítés lefoglalt példány esetén**

Ha vissza kell térítenie egy foglalást, válassza a **Foglalás részletei gombra,** majd a Visszatérítés **gombra kattintva.**

**Pro-rated visszatérítés:**

**Pro-ration and minimum requirement examples for refund and exchange** Példa előzetes foglalásra:

- Január 1-jén 120 USD-ért vásárol egy éves ri ri-t
- Április 7-én vissza szeretné téríteni vagy cserélni a foglalást
- Mivel a foglalás 97 napja élőben van, ön (1-97/365) * 120 USD-t kap vissza. (azaz 88,1 USD). A visszatérítések jelenleg nem aktívak.
- Csere esetén az új vásárlásnak nagyobbnak kell lennie, mint 88,1 USD
- Jelenleg nem áll rendelkezésre pénzvisszatérítés.

**Példa a számlázási csomag foglalási példára:**

- Egyéves ri-t vásárol 10 USD-ért havonta
- Április 7-én vissza szeretné téríteni vagy cserélni a foglalást
- Mivel az utolsó fizetés 7 nap volt, ön (1-7/31) * 10 USD-t kap vissza. (azaz 774 Ft)
- A jövőbeli törölt kifizetések 80 USD- A visszatérítések jelenleg nem aktívak.
- Ez a lemondás 87,74 USD-t von vissza Öntől az 50 000 USD visszatérítési korlátról.
- Csere esetén az új vásárlás teljes értékének nagyobbnak kell lennie, mint 87,74 USD

**Nem látható a legutóbbi számlázási időszak számlája**

Néhány lehetséges ok, amiért esetleg nem látható a számla:

- Olyan havi kreditet kap az előfizetésével, amely nem lépte túl, vagy ingyenes próbaverzióval rendelkezik. Egy számla csak akkor jön létre, ha Ön tartozásból
- Kevesebb mint 30 nap van attól a naptól, amikor előfizetett az Azure-ra.
- A számla még nem jön létre. Várakozás a számlázási időszak végéig
- Ha nem Ön a fiók adminisztrátora, előfordulhat, hogy a régebbi számlák nem érhetők el

**A számla letöltése az Azure Portalról (.pdf)**

- Válassza ki előfizetését az Azure Portal [Előfizetések](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) lapján, felhasználóként, aki [hozzáfér a számlákhoz.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Select **Invoices**
- Kattintson **a Számla letöltése** elemre a PDF-számla másolatának megtekintéséhez. Ha a Nem érhető el lehetőség **látható,** tekintse meg a Miért nem látom a legutóbbi számlázási időszak [számláját?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Számla fogadása e-mailben (.pdf)**

- Válassza ki előfizetését az [Előfizetések lapon.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Kattintson **a Számlák, majd** a Saját számla küldése e-mailben elemre.
- Kattintson **az opt in (opt in) gombra,** és fogadja el a feltételeket. Minden előfizetéséhez külön-külön be kell jelentkeznie

Megjegyzés: Ha a lépések után nem kap e-mailt, ellenőrizze, hogy helyes-e az e-mail-cím a profil kommunikációs [beállításai között](https://account.windowsazure.com/profile)

**Használati adatok letöltése az Azure Portalról**

- Bejelentkezés az [Azure Fiókközpontba](https://account.windowsazure.com/Subscriptions) [fiók-rendszergazdaként](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Válassza ki azt az előfizetést, amelynek a számláját és a használati adatait meg szeretné tudni
- Számlázási **előzmények kiválasztása**
- Válassza **az Aktuális utasítás megtekintése lehetőséget** a becsült díjak becsült értékének megtekintéséhez a becslés generálásakor.
- Válassza **a Használat letöltése lehetőséget** a napi használati adatok CSV-fájlként való letöltéséhez. Ha két elérhető verzió látható, töltse le a 2-es verziót

További kérdések: [Fenntartott példányok dokumentumok felkeresve](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ajánlott dokumentumok**

- [Számlázási alapismeretek](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A fenntartott példányra érvényes árengedmény alkalmazása](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Az Azure számlázási számlájának és napi használati adatainak letöltése vagy megtekintése](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A fenntartott példányra érvényes árengedmény alkalmazása](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A "Pay-As-You-Go" előfizetéshez lefoglalt példányhasználat](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A nagyvállalati regisztrációhoz lefoglalt példányhasználat](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A foglalt példányok nem tartalmazzák a Windows szoftverköltségeket](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Fenntartott példányok a Partner Central Cloud Solution Provider (CSP) programban](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)