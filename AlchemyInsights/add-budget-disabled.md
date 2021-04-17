---
title: Miért van letiltva a Költségvetés hozzáadása gomb?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822637"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Miért van letiltva a Költségvetés hozzáadása gomb?

Költségvetés létrehozásához az alábbi engedélyek valamelyikére van szükség:

- Management Group, Subscription, Resource Group Scopes
- Költségkezelési munkatárs
- Tulajdonos
- Közreműködő
- Csak nagyvállalati ügyfél esetén: Regisztráció, Részleg, Fiókhatókörök
- Regisztrációs rendszergazda (költségvetés beállítása a Regisztráció hatókörében)
- Részleg rendszergazdája (költségvetés beállítása a részleg hatókörében)
- Fióktulajdonos (költségvetés beállítása a fiók hatókörében)
- Csak modern ügyfélszerződés: Számlázási fiók, számlázási profil, számlaszakaszok hatóköre
- Azure-előfizetés létrehozója

**Létrehozottam egy költségvetést, amikor az aktuális hónapra vonatkozó költség már túl lett kért. Miért nem tudok riasztást kapni?**  
Ha a költségvetés létrehozásakor már túllépte a megadott küszöbértéket, akkor a riasztás nem lép hető fel. Ha egy új ciklus kezdődik, és megszegi a küszöbértéket, a riasztás kigyullad.

**Mikor számíthatok riasztásra, ha túllépem valamelyik tervezett riasztási küszöbértékemet?**  
A költségvetések kiértékelése 4 óránként történik. A használati adatoknak legalább 8 óra alatt el kell érnie a költségvetési rendszert. A riasztások így akár 12 órát is igénybe vehetnek, miután túllépte a küszöbértéket.

**Miért van letiltva a Kezdő dátum gomb a Hónap vagy a Számlázás hónap alaphelyzetbe állítási időszakának kiválasztásakor?**  
A költségvetések az aktuális naptári hónaphoz vagy az aktuális számlázási időszakhoz vannak igazítva (ebben az esetben a Számlázási hónap beállítás van kiválasztva). Ezért ezt az értéket előre kitöltjük Önnek.

**Miért nem látom a költségek grafikont a költségvetés-létrehozási élményben?**  
Legalább 2 hónapos költségadatra van szükségünk ahhoz, hogy megjelenítsünk egy grafikont, amely segíti a költségvetés létrehozását.

**Miért nem tudok költségvetést beállítani egy éppen létrehozott előfizetéshez?**  
Az előfizetés létrehozása után az adatok feldolgozása 24–48 órát vesz igénybe, mielőtt költségvetést hoz létre hozzá.

**Budget API Resources**

- [Budgets API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Műveleteket biztosít a költségvetések létrehozásához és frissítéséhez. A KöltségvetésEK API-val beállíthatja a költségvetés küszöbértékét, és több riasztást is konfigurálhat a küszöbérték beállításakor. A riasztások elindíthatja az e-maileket vagy az Azure-műveletcsoportokat automatizálási műveletek elvégzéséhez. Megjegyzés: Az API-hoz való szűrés nem igazodik a Lekérdezési API szűrési és dimenzióihoz.
- [Budgets API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Hozzon létre költségvetéseket a v1-esnél nagyobb költségszűrési lehetőségekkel. A szűrés igazodik a Lekérdezés és a Dimenzió API-kban használt szerződéshez. Ez a tovább való használathoz ajánlott költségvetési API.
- [Dimenziók:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Műveleteket biztosít a különböző hatókörök szerinti használat támogatott dimenzióinak lekérthez. A Dimenziók API használatával lekérheti a dimenziók listáját, amelyek a Lekérdezés API-val lekérdezések létrehozásához használhatók.
- [Lekérdezés:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Műveleteket biztosít az összesített költség- és használati adatok be szerezni a lekérdezés alapján. A lekérdezési API-val megadhatja a kívánt szűrési, rendezési és csoportosítási beállításokat az összes elérhető dimenzió szerint (ezek a Méretek API-ból érhetők el).

**Előre jelzett költségek**

**Miért nem látom a költségek előrejelzését a Költségelemzésben?**  
Több oka is lehet annak, ha az előrejelzési előrejelzés hiányzik a Költségelemzés eszközből, ezek némelyike a következő:

1. Ha a költségadatok kevesebb mint 10 naposak, az előrejelzési diagram nem töltődik be. A modellhez legalább 10 nap friss költségadat szükséges a pontos előrejelzéshez.
2. Ha régi dátumokat jelölt ki, akkor az előrejelzési diagram nem lesz látható. Válasszon egy jövőbeli dátumokat megjelenítő dátumtartományt az előrejelzési diagram megjelenítéséhez
3. Ha a számla pénzneme több, az előrejelzési diagramon csak a "Minden költség USD-

**Miért nem változik meg az előrejelzés az erőforrások módosításakor?**  
Az előrejelzési modellnek néhány napig kell figyelembe vennie a fiók változásait, és nem vet ki azonnali előrejelzést az erőforrások változásai alapján.  
Az erőforrások növelésének vagy csökkentésének nagyobb lépései esetén a modellhez kissé tovább fog tartani a módosításokhoz való igazodás, hogy figyelembe vegye az eltéréseket.

**Miért növeli az előrejelzésem a foglalás vagy a Piactér megvásárlását követően?**  
Az előrejelzési modell figyelembe veszi az Ön tényleges költségét, és nem veszi figyelembe külön a használatot és a vásárlást. Az egyszer megvásárolható modell 10 nap után csökkenti a kivetítéseket, hogy figyelembe véve a költségek hirtelen növekedését

**Egyetlen dimenzióra (például) vonatkozó előrejelzéseket szeretnék látni Méter)**  
Az előrejelzés jelenleg nem egyedi méterenként, de teljes költségvetületeket támogat. Ezért ha a "Csoportosítás" dimenzió szerint történik, akkor a kivetítés a dimenzió összes tételének összege lesz.

**Ajánlott dokumentumok**

- [Mi az Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Ajánlott eljárások az Azure Költségkezeléshez](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Költségek és kiadások elemzése](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Költségek feltárása és elemzése költségelemzéssel](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Díjszabás](https://azure.microsoft.com/services/cost-management/#pricing)
- [Költségek áttekintése a költségelemzésben](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Oktatóvideó: Költségvetés létrehozása az Azure Portalon](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [A költségvetések megtekintésének és testreszabásának előfeltételei](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Költségvetések létrehozása és kezelése](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Automatizálás konfigurálása az Azure Action Groups és Budgets API-val](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Használati és kiadások figyelése költségriasztásokkal](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Ajánlott eljárások költségkezeléshez](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Oktatóvideók**

- [Költségvetés létrehozása az Azure Portalon](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Költségek kezelése a Költségvetés API-val és a műveletcsoportokkal](https://go.microsoft.com/fwlink/?linkid=2147038)