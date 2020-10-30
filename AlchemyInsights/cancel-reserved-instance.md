---
title: Foglalás lemondása
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807571"
---
# <a name="cancelling-reservation"></a>Foglalás lemondása

- Önkiszolgáló **:** A fenntartott példányokat az [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)segítségével is lemondhatja vagy cserélheti. Jelölje ki a foglalást, és kattintson a visszatérítés vagy az Exchange elemre. Felhívjuk a figyelmét arra, hogy a foglalási sorrendben tulajdonosi hozzáféréssel kell rendelkeznie az Exchange-hez vagy a visszatérítéshez. A csak a foglalásokhoz való hozzáférés nem teszi lehetővé a visszatérítést vagy az Exchange-et. A foglalási rendelés tulajdonosának felkérése, hogy tulajdonosi hozzáférést adjon a foglalási rendeléshez
- **Exchange-házirend:** Egy másik, azonos típusú foglalásra szóló foglalást kicserélheti – nincsenek **szankciók** a foglalási cserében. Az új fenntartással való teljes kötelezettségvállalásnál nagyobbnak kell lennie, mint a kicserélt foglalások összege és a jövőbeli havi kifizetések (ha szükséges)
- **Visszatérítési szabály:** A visszatérítés összege és a lemondott jövőbeli kifizetések száma nem haladhatja meg a $50 000 USD-t egy 12 hónapos gördülési ablakban. Jelenleg nem számítunk fel **semmilyen szankciót** a visszatérítésekre, de a jövőbeli pénzvisszatérítések esetében nem.  
    **Kivételek:** Az önkiszolgáló Exchange és a Mégse lehetőség nem érhető el az Amerikai Egyesült államokbeli kormányzati Enterprise szerződés ügyfelei számára
- Az **API/PS/CLI** támogatás nem áll rendelkezésre a lemondáshoz és [a](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) visszatérítésekhez
- Az önkiszolgáló Exchange és a Mégse lehetőség nem érhető el az Amerikai Egyesült államokbeli kormányzati vállalati szerződés ügyfelei számára. A többi amerikai kormányzati verzió előfizetése, többek között a fizetés-kirovó és a CSP támogatása

További információ: [a visszatérési és az Exchange-tranzakciók feldolgozása](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
További információ: [az Exchange-és visszatérítési házirendek](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Egyéb kérdések: a [fenntartott példányokra vonatkozó dokumentumok meglátogatása](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Meglévő fenntartott példány cseréje (önkiszolgáló)**

Megoszthatja a foglalásokat egy másik, azonos típusú foglaláshoz. Ha már nincs szüksége rá, a foglalást visszafizetheti, az $50 000 USD-ig évente. Az önkiszolgáló Exchange és a Mégse lehetőség nem érhető el az Amerikai Egyesült államokbeli kormányzati vállalati szerződés ügyfelei számára. A többi amerikai kormányzati verzió előfizetése, többek között a fizetés-kirovó és a CSP is támogatott. Egy meglévő foglalás cseréjéhez vagy visszafizetéséhez tulajdonosi hozzáféréssel kell rendelkeznie a foglalási sorrendben.

Az alábbi lépések végigvezetik a tranzakció befejezésének lépésein.

1. Jelentkezzen be az [Azure-portálra](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Jelölje ki a visszatéríteni kívánt foglalásokat, és kattintson az **Exchange** elemre.
2. Jelölje ki a megvásárolni kívánt VM-terméket, és írjon be egy mennyiséget. Győződjön meg arról, hogy az új beszerzési összeg nagyobb, mint a [vásárlást megelőző](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy) végösszeg
3. A tranzakció véleményezése és befejezése

**A lefoglalt példány visszatérítése**

A foglalás visszafizetéséhez válassza a **foglalás részletei** lehetőséget, és kattintson a **visszatérítés** gombra.

**Pro névleges visszatérítés:**

**A pénzértékek és a minimális követelmény a visszatérítés és az Exchange esetében**  
Példa előzetes foglalásra:

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

**Ajánlott dokumentumok**

- [A visszatérési és az Exchange-tranzakciók feldolgozása](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Exchange-és visszatérítési házirendek](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)