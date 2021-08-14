---
title: Foglalás lemondása
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
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931235"
---
# <a name="cancelling-reservation"></a>Foglalás lemondása

- **Önkiszolgáló szolgáltatás:** Saját maga is lemondhatja vagy kicserélheti a fenntartott példányokat az [Azure Portal használatával.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Jelölje ki a foglalást, és kattintson a visszatérítésre vagy a csere elemre. Felhívjuk a figyelmét arra, hogy tulajdonosi hozzáféréssel kell rendelkezik a foglalási rendeléshez a csere vagy visszatérítés érdekében. Kizárólag a Foglaláshoz való hozzáférés esetén nem jogosult visszatérítésre vagy cserére. Kérje meg a foglalási rendelés tulajdonosát, hogy adjon Önnek hozzáférést a foglalási rendeléshez.
- **Exchange házirend:** Más, azonos típusú foglalások lefoglalását is át lehet cserélni – a foglalási csere nem tartalmazza **a** szobafoglalási összeget. Az új foglalással kapcsolatos teljes kötelezettségvállalásnak nagyobbnak kell lennie, mint az átváltott foglalások visszatérítési összege és a jövőbeli havi kifizetések összege (ha van ilyen).
- **Visszatérítési szabályzat:** A visszatérítés összege és a lemondott jövőbeli kifizetések nem haladhatja meg az 50 000 usd-t egy 12 hónapos görgető ablakban. Jelenleg nem **számolunk fel** pénzvisszatérítési díjat, de a jövőbeli visszatérítések után rá lehet fizetni.  
    **Kivételek:** Az önkiszolgáló csere- és lemondási funkció nem érhető el az Egyesült Egyesült kormányzati ügyfeleinek Nagyvállalati Szerződés számára
- **Az API/PS/CLI** támogatása nem érhető el lemondáshoz és visszatérítéshez Önkiszolgáló tőzsdére és visszatérítésre [Azure-foglalások esetén](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Az önkiszolgáló csere- és lemondási funkció nem érhető el az Egyesült Államok kormányzati ügyfelei Nagyvállalati Szerződés számára. Más, egyesült egyesült államokkal kapcsolatos előfizetési típusok, például a "Fizetés mint Ön-go" és a "CSP" támogatottak

További információ: [A visszaküldési és a cseretranzakciók feldolgozása](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
További információ: [Exchange és visszatérítési szabályzatok](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
További kérdések: [Fenntartott példányok dokumentumok felkeresve](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange lefoglalt példány (Önkiszolgáló)**

Ugyanezen típusú más foglalások foglalását is kicserélheti. Ha már nincs rá szüksége, visszatéríthet egy 50 000 USD összeget is évente. Az önkiszolgáló csere- és lemondási funkció nem érhető el az Egyesült Államok kormányzati ügyfelei Nagyvállalati Szerződés számára. Az Egyesült Államok kormányzati előfizetési típusai, például a "Pay-As-You-Go" és a "CSP" előfizetések támogatottak. A meglévő foglalások cseréjéhez vagy visszatérítésére tulajdonosi hozzáféréssel kell lennie a foglalási rendelésben.

Az alábbi lépések végigvezetik a tranzakció befejezésének eljárásán.

1. Jelentkezzen be az [Azure Portalba.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Jelölje ki a visszatérítendő foglalásokat, és kattintson **a** Exchange
2. Válassza ki a megvásárolni kívánt VM-terméket, és írjon be egy mennyiséget. Ügyeljen arra, hogy az új vásárlási összeg nagyobb legyen, mint a vissza visszaút [összege:](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy) A megfelelő méret meghatározása vásárlás előtt
3. A tranzakció áttekintése és befejezése

**Visszatérítés lefoglalt példány esetén**

Ha vissza kell térítenie egy foglalást, válassza a **Foglalás részletei gombra,** majd a Visszatérítés **gombra kattintva.**

**Pro-minősítésű visszatérítés:**

**Pro visszatérítésre és cserére vonatkozó minimális követelmény**  
Példa előzetes foglalásra:

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

**Ajánlott dokumentumok**

- [A visszaküldési és a cseretranzakciók feldolgozásának folyamata](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Exchange és visszatérítési szabályzatok](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)