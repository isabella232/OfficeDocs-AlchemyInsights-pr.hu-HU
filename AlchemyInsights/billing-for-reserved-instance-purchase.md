---
title: Számlázás a lefoglalt példányok vásárlásakor
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
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823077"
---
# <a name="billing-for-reserved-instance-purchase"></a>Számlázás a lefoglalt példányok vásárlásakor

A lefoglalt példány beszerzése a vásárlás időpontjában kiválasztott előfizetéshez kötött fizetési módra terheli. Az előfizetés típusa vállalati szerződés (ajánlati szám: MS-AZR-0017P), Pay-as-go (ajánlati szám: MS-AZR-0003P), Microsoft ügyfél-szerződés vagy CSP.

- Nagyvállalati verziós előfizetés esetén a díjakat a program levonja a beiratkozási pénzügyi egyenlegből vagy a túlóradíjra.
- A fizetés-kirovó előfizetés esetén a díjakat a hitelkártyára vagy az előfizetés számlájának fizetési módjára kell kiszámlázni.

**Foglalás lemondása**

- Önkiszolgáló **:** A fenntartott példányokat az [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)segítségével is lemondhatja vagy cserélheti. Jelölje ki a foglalást, és kattintson a visszatérítés vagy az Exchange elemre. Felhívjuk a figyelmét arra, hogy a foglalási sorrendben tulajdonosi hozzáféréssel kell rendelkeznie az Exchange-hez vagy a visszatérítéshez. A csak a foglalásokhoz való hozzáférés nem teszi lehetővé a visszatérítést vagy az Exchange-et. A foglalási rendelés tulajdonosának felkérése, hogy tulajdonosi hozzáférést adjon a foglalási rendeléshez
- **Exchange-házirend:** Egy másik, azonos típusú foglalásra szóló foglalást kicserélheti – nincsenek **szankciók** a foglalási cserében. Az új fenntartással való teljes kötelezettségvállalásnál nagyobbnak kell lennie, mint a kicserélt foglalások összege és a jövőbeli havi kifizetések (ha szükséges)
- **Visszatérítési szabály:** A visszatérítés összege és a lemondott jövőbeli kifizetések száma nem haladhatja meg a $50 000 USD-t egy 12 hónapos gördülési ablakban. Jelenleg nem számítunk fel **semmilyen szankciót** a visszatérítésekre, de a jövőbeli pénzvisszatérítések esetében nem.

**Kivételek:** Az önkiszolgáló Exchange és a Mégse lehetőség nem érhető el az Amerikai Egyesült államokbeli kormányzati Enterprise szerződés ügyfelei számára

- Az **API/PS/CLI** támogatás nem áll rendelkezésre a lemondáshoz és [a](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) visszatérítésekhez
- Az önkiszolgáló Exchange és a Mégse lehetőség nem érhető el az Amerikai Egyesült államokbeli kormányzati vállalati szerződés ügyfelei számára. A többi amerikai kormányzati verzió előfizetése, többek között a fizetés-kirovó és a CSP támogatása

További információ: [a visszatérési és az Exchange-tranzakciók feldolgozása](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) : További kérdések [az Exchange és a visszatérítés szabályairól: a](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) [fenntartott példányokra vonatkozó dokumentumok megkeresése](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Meglévő fenntartott példány cseréje (önkiszolgáló)**

Megoszthatja a foglalásokat egy másik, azonos típusú foglaláshoz. Ha már nincs szüksége rá, a foglalást visszafizetheti, az $50 000 USD-ig évente. Az önkiszolgáló Exchange és a Mégse lehetőség nem érhető el az Amerikai Egyesült államokbeli kormányzati vállalati szerződés ügyfelei számára. A többi amerikai kormányzati verzió előfizetése, többek között a fizetés-kirovó és a CSP is támogatott. Egy meglévő foglalás cseréjéhez vagy visszafizetéséhez tulajdonosi hozzáféréssel kell rendelkeznie a foglalási sorrendben.

Az alábbi lépések végigvezetik a tranzakció befejezésének lépésein.

1. Jelentkezzen be az [Azure-portálra](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Jelölje ki a visszatéríteni kívánt foglalásokat, és kattintson az **Exchange** 2 elemre. Válassza ki a MEGVÁSÁROLNI kívánt VM-terméket, és írjon be egy mennyiséget. Győződjön meg arról, hogy az új beszerzési összeg nagyobb, mint a [vásárlás után](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)a teljes összeg.
3. a tranzakció áttekintése és befejezése

**A lefoglalt példány visszatérítése**

A foglalás visszafizetéséhez válassza a **foglalás részletei** lehetőséget, és kattintson a **visszatérítés** gombra.

**Pro névleges visszatérítés:**

A pénzértékek **és a minimális követelmény a visszatérítés és az Exchange esetében** Példa előzetes foglalásra:

- Január 1-jén vásárol egy éves időszakot az $120-hoz
- Április 7-én szeretné visszatéríteni vagy lecserélni a foglalást
- Mivel a foglalás 97-es napokra van megnyitva, az (1-97/365) * $120 vissza fog lépni. (például $88,1). A visszatérítésekre jelenleg nincs büntetés
- Ha a csere, az új vásárlásnál nagyobbnak kell lennie, mint a $88,1
- Jelenleg nincs bírság a visszatérítésekre

**Példa számlázási terv foglalására:**

- Az $10 havonta vásárol egy egyéves időszakot
- Április 7-én szeretné visszatéríteni vagy lecserélni a foglalást
- Mivel a legutóbbi fizetés 7 napig megtörtént, az (1-7/31) * $10 vissza fog történni. (azaz $7,74)
- A jövőbeli kifizetések lemondása a $80. A visszatérítésekre jelenleg nincs büntetés
- Ez a törlés levonja az $87,74-öt az $50 000-ös visszatérítési korlátból.
- Ha a csere, az új vásárlás teljes értéke nem lehet nagyobb, mint $87,74

**Nem jelenik meg az utolsó számlázási időszak számlája**

Bizonyos okok miatt előfordulhat, hogy nem jelenik meg számla:

- Az előfizetésével egy vagy több ingyenes próbaverzióval rendelkezik. A számla csak akkor jön létre, amikor pénzt köszönhet
- Az Azure-ra előfizetett naptól számított 30 napnál rövidebb
- A számla még nincs létrehozva. Várakozás a számlázási időszak végére
- Ha nem a fiók rendszergazdája, előfordulhat, hogy a régebbi számlák nem érhetők el Önnek

**A számla letöltése az Azure portálról (. pdf)**

- Válassza ki az előfizetését az Azure Portal [előfizetések](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) lapjáról a [számlákhoz való hozzáférésre szolgáló felhasználóként](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- **Számlák** kijelölése
- A PDF-számla másolatának megtekintéséhez kattintson a **számla letöltése** parancsra. Ha az **nem érhető** el, olvassa el [a miért nem jelenik meg az utolsó számlázási időszak számlája?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice) című témakört.

**A számla vétele e-mailben (. pdf)**

- Válassza ki az előfizetést az [előfizetések](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) lapról. Kattintson a **számlák** , majd a számla küldése e-mailben lehetőségre
- Kattintson **a választás gombra, és** fogadja el a feltételt. Mindegyik előfizetés esetén be kell jelentkeznie.

Megjegyzés: Ha a lépések követése után nem kap e-mailt, ellenőrizze, hogy helyes-e az e-mail-cím a [profil kommunikációs beállításai](https://account.windowsazure.com/profile) között

**A használati adatainak letöltése az Azure portálról**

- Bejelentkezni az [Azure Account Center](https://account.windowsazure.com/Subscriptions) -be a [fiók rendszergazdája](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Jelölje ki azt az előfizetést, amelynek a számláját és a használati adatait meg szeretné jeleníteni.
- **Számlázási előzmények** kijelölése
- Válassza a **jelenlegi utasítás megtekintése** lehetőséget, ha a becslést a díj létrejöttének időpontjában szeretné megjeleníteni.
- Válassza a **használat letöltése** lehetőséget a napi használati adatainak CSV-fájlként való letöltéséhez. Ha két verzió érhető el, töltse le a 2-es verziót

Egyéb kérdések: a [fenntartott példányokra vonatkozó dokumentumok meglátogatása](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ajánlott dokumentumok**

- [Számlázás alapjai](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A lefoglalt példány kedvezményének ismertetése](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Az Azure számlázási számlájának és a napi használati adatainak letöltése vagy megtekintése](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A lefoglalt példány kedvezményének ismertetése](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A lefoglalt példány felhasználásának ismertetése a fizetési mód előfizetése során](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A lefoglalt példány használatáról a nagyvállalati verziós igénylésekre vonatkozóan](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A Windows szoftver azon költségei, amelyek nem szerepelnek a lefoglalt példányokban](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Fenntartott példányok a fiókpartner központi felhőalapú megoldás-szolgáltatójában (CSP-es program)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)