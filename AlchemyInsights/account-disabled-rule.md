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
ms.openlocfilehash: 8918b0da0172e0421ade6f0cca936e14d1d609896bc4c75c5a8491c0dbe75aff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938445"
---
# <a name="azure-subscription-disabled"></a>Azure-előfizetés letiltva

Azure-előfizetését letilthatja, ha lejárt a kreditje, elérte a költségkeretet, lejárt a számla, eléri a hitelkártyás korlátot, vagy lemondta az előfizetést a fiók rendszergazdája. Alább arról olvashat, hogy miként engedélyezheti újra előfizetését. További információ: [Azure-előfizetés újraaktiválása](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support)

**Azure-előfizetés újra engedélyezése (az előfizetést véletlenül megszüntették)** A [fiók rendszergazdája](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) újraaktiválhat egy lemondott "Go-ként" előfizetést az Fiókközpontban:

1. Jelentkezzen be a [Fiókközpontba.](https://account.windowsazure.com/Subscriptions)
2. Válassza ki a lemondott előfizetést. Kattintson **az Újraaktiválás gombra.**

Más előfizetési típusok esetén lépjen [kapcsolatba az ügyfélszolgálattal](https://portal.azure.com/?#blade/Microsoft_Azure_Support/HelpAndSupportBlade) az előfizetés újraaktiválásához.

**Lejárt hitelkártya**

Ha regisztrál egy **ingyenes** Azure-fiókra, kap egy ingyenes próba-előfizetést, amely 200 USD-s Azure-krediteket biztosít 30 napra és 12 hónap ingyenes szolgáltatásokra. 30 nap végén az Azure letiltja az előfizetését. Az előfizetés le van tiltva, hogy megvédje az előfizetésében szereplő krediten és ingyenes szolgáltatásokon túli használati díjaktól. Az Azure-szolgáltatások használatának folytatásához frissítenie kell [az előfizetését.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support) A frissítés után az előfizetése 12 hónapig továbbra is hozzáfér az ingyenes szolgáltatásokhoz. Az ingyenes szolgáltatásokon és mennyiségeken kívül csak az ingyenes szolgáltatásokért és mennyiségekért számítunk fel díjat.  
További információ: [Lejárt hitelkártya](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support#your-credit-is-expired)

**Elérte a korlátot**

Amikor a használat eléri a költségkeretet, az Azure a számlázási időszak hátralévő részére letiltja az előfizetést. Az előfizetés le van tiltva, hogy megvédje az előfizetésében szereplő jóváíráson túli használati díjak véletlen kiírását. Ha el szeretné távolítani a költségkeretet, tekintse meg az [Azure költségkeretét.](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)  
További információ: [Elérte a költségkeretet](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled?WT.mc_id=Portal-Microsoft_Azure_Support#you-reached-your-spending-limit)

**Esedékes számla**

A hátralékos egyenleg feloldásáról az Azure-előfizetésen túli esedékes összeg feloldása az [Azure-ból e-mail-cím beszerzése után.](https://docs.microsoft.com/azure/billing/billing-azure-subscription-past-due-balance?WT.mc_id=Portal-Microsoft_Azure_Support)

**A számla túllépi a hitelkártyás korlátot**

A probléma megoldásához [váltson át egy másik hitelkártyára.](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support) Vagy ha egy vállalkozást képvisel, számlával is [fizethet.](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)

**Megjegyzés:** Az újra engedélyezett előfizetések egy új előfizetési évfordulós dátumot fognak hozzárendelni. Az előfizetés felfüggesztésének időtartama (intervalluma) hozzá lesz adva az eredeti sa dátumhoz. Ha az évforduló 29., 30. vagy 31. napja esik, akkor a sa dátum a következő hónap 1-jára lesz beállítva.  
Példa:

- Az eredeti előfizetési évfordulója 25.
- Az előfizetést január 3-án felfüggesztettük, és 2009. 10-én újra engedélyezték;
- Az előfizetést 6 napig letiltották (6-os intervallum);
- A rendszer ezután hozzáadja az időközt az eredeti sa-hez, és az összeg lesz az új Sa dátum (25+6=31). 

**Megjegyzés:** Ebben a példában, mivel a Sa dátum mostantól nagyobb, mint 28, az új Sa dátum a következő hónap első dátuma lesz.

**Ajánlott dokumentumok**

- [Előfizetésváltás](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [Előfizetés lemondása](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [Azure Piactér](https://azuremarketplace.microsoft.com/marketplace/?source=datamarket)
- A [fiók-rendszergazda megkeresi](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- [Mit tegyek, ha az Azure-előfizetésemet letiltják?](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure-költési korlát](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)
