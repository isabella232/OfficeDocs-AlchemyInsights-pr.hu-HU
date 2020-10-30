---
title: Miért le van tiltva a költségvetés hozzáadása gomb?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807410"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Miért le van tiltva a költségvetés hozzáadása gomb?

Költségvetés létrehozásához az alábbi engedélyek egyikére van szükség:

- Felügyeleti csoport, előfizetés, erőforráscsoport-hatókörök
- Cost Management munkatárs
- Tulajdonos
- Közreműködői
- Csak nagyvállalati ügyfél: beiratkozási, Részlegi, fiók-hatókörök
- Beiratkozási rendszergazda (költségvetés beállítása a beiratkozási hatókörben)
- Department admin (költségvetés beállítása a részleg hatókörében)
- Fiók tulajdonosa (költségvetés beállítása a fiók hatókörében)
- Csak modern ügyfél-szerződés: számlázási fiók, számlázási profil, számla szakasz hatókörök
- Azure előfizetés-készítő

**Létrehozott egy költségvetést, ha az aktuális hónapra vonatkozó költségem már túl volt a költségvetésben. Miért nem kaptam figyelmeztetést?**  
Ha már túllépte a megadott költség küszöböt, ha olyan költségvetést hoz létre, amelyet a riasztás nem fog tüzet. Ha megszegi a küszöböt, az új ciklus megkezdése után a riasztás tüzet fog látni.

**Mikor kell figyelmeztetést kapni arra az esetre, ha túlléptem a meghatározott költségvetés-riasztási küszöbök egyikét?**  
A költségvetés 4 óránként kerül kiértékelésre. A használati adatok eléréséhez legalább 8 óra szükséges a költségvetések rendszeréhez. Tekintettel arra, hogy a határértékek túllépése után a riasztások akár 12 órát is igénybe vehetnek.

**Miért van letiltva a kezdési dátum gomb, amikor kijelölek egy hónap vagy számlázási hónap reset időszakot?**  
A költségvetések az aktuális naptári hónaphoz vagy az aktuális számlázási időszakhoz igazodnak (abban az esetben, ha a számlázási hónap elem van kiválasztva). Így előre kitöltjük ezt az értéket.

**Miért nem látható a költségeim grafikonja a költségvetés-készítési felületen?**  
Ahhoz, hogy a diagramot a költségvetés létrehozásakor segítse, legalább 2 hónapig kell lennie a költség adatoknak.

**Miért nem tudok költségvetést beállítani az imént létrehozott előfizetéshez?**  
Az előfizetés létrehozása után az 24-48 órákba telik, amíg a költségvetést nem állítja be.

**Költségvetési API-források**

- [Költségvetés API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): a költségvetések létrehozására és frissítésére szolgáló műveleteket nyújt. A költségvetés API-t használva megadhat egy költségvetési küszöböt, és több riasztást is beállíthat, miközben a küszöböt közelíti meg. Az értesítésekkel elindíthat egy e-mailt vagy egy Azure-műveleti csoportot az automatizálás végrehajtásához. Megjegyzés: az API szűrése nem igazodik a Query API szűrési és méretekkel.
- [Költségvetés API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): költségvetések létrehozása nagyobb költség-szűrési lehetőségekkel, mint a v1. A lekérdezésben és a méretek API-ban használt szerződéshez igazítja a szűrést. Ez az ajánlott költségvetés API a továbblépés használatához.
- [Dimenziók](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): a különböző hatókörökhöz tartozó támogatott méretek elérésére szolgáló műveleteket nyújt. A Dimensions API segítségével megkeresheti azokat a dimenziókat, amelyek bemenetként használhatók a Query API-val való lekérdezések generálásához.
- [Lekérdezés](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): a megadott lekérdezés alapján összesített költség-és használati adatokat jelenít meg. A lekérdezési API-t használva megadhatja a kívánt szűrést, rendezést és csoportosítást az összes elérhető dimenzión (amely a dimenziók API-val érhető el).

**Előrejelzett költségek**

**Miért nem látom az előrejelzéseket a költség-elemzés költségei között?**  
Több oka lehet annak, ha az előrejelzési vetületek a költség-elemzésben hiányoznak, néhányuk az alábbiak szerint történik:

1. Ha a költség adatértéke 10 napnál régebbi, akkor az előrejelzési diagram nem töltődik be. A modellnek a pontos előrejelzésekhez legalább 10 napig kell bemutatnia a legutóbbi költséget.
2. Ha a történelmi dátumok lehetőséget választotta, akkor az előrejelzési diagram nem jelenik meg. Adja meg a dátumtartományt az előrejelzési diagram jövőbeli dátumait tartalmazó dátumtartomány megadásához.
3. Ha a fiókja több pénznemet tartalmaz, az előrejelzési diagram csak az "USD-es költség" projekt költségeit fogja tartalmazni.

**Miért nem változik az előrejelzés, ha módosításokat végezek az erőforrások között?**  
Az előrejelzési modellnek több napra van szüksége a fiók változásainak elvégzéséhez, és nem lehet az erőforrásokban való változáson alapuló azonnali előrejelzések  
Ha nagyobb mértékben szeretné növelni vagy csökkenteni az erőforrásokat, a modell kissé tovább fog tartani ahhoz, hogy ezek a változások figyelembe vegyék a rendellenességeket

**Miért jelenik meg az előrejelzésem a foglalás vagy a piactér vásárlása után?**  
Az előrejelzési modell a tényleges költséget veszi figyelembe, és nem veszi figyelembe a használatot és a vásárlást külön-külön. Egyszeri vásárlás esetén a modell 10 nap elteltével csökkenti a prognózist a költségek hirtelen emelkedésének figyelembevétele érdekében.

**Szeretném megtekinteni az előrejelzéseket egyetlen dimenzióra (például. Állapotjelzője**  
Az előrejelzés jelenleg a teljes költség előrejelzését támogatja, az egyes mérőórák esetében nem. Így, ha egy dimenzió szerint csoportosítva van, a kivetítések a dimenzióban szereplő összes elem összegét fogják tartalmazni.

**Ajánlott dokumentumok**

- [Mi az Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gyakorlati tanácsok az Azure Cost-kezeléshez](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A költségek és a kiadások elemzése](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [A költség-elemzés költségeinek feltárása és elemzése](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure költség-kezelés: árak](https://azure.microsoft.com/services/cost-management/#pricing)
- [A költség-elemzés költségeinek áttekintése](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Videó oktatóprogram: költségvetés létrehozása az Azure portálon](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Költségvetések megtekintéséhez és testreszabásához szükséges előfeltételek](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Költségvetések létrehozása és kezelése](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Az automatizálás beállítása az Azure műveleti csoportokkal és a költségvetések API-val](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Használati és kiadások figyelése a Cost riasztásokkal](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gyakorlati tanácsok a Cost-kezeléshez](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Oktatóanyagok a videókhoz**

- [Költségvetés létrehozása az Azure portálon](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Költségek kezelése a költségvetés API-val és a műveleti csoportokkal](https://go.microsoft.com/fwlink/?linkid=2147038)