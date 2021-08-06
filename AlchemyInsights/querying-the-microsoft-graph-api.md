---
title: A Microsoft Graph API lekérdezése
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
- "9004345"
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923241"
---
# <a name="querying-the-microsoft-graph-api"></a>A Microsoft Graph API lekérdezése

Ez a témakör azokra a fejlesztőkre is vonatkozhat, akik továbbra is az Azure AD Graph API-t használják. Azonban erősen  ajánlott a Microsoft Graph használata az összes címtár-, identitás- és hozzáférés-kezelési esethez.

**Hitelesítési vagy engedélyezési problémák**

- Ha az  app nem tud jogkivonatokat szerezni a Microsoft Graph hívásához, válassza a Probléma a hozzáférési jogkivonat **(hitelesítés)** Microsoft Graph kategóriával, és további segítséget és támogatást kap erről a témakörről.
- Ha appja **401-es vagy 403-as** engedélyezési hibát kap a Microsoft Graph hívása közben, a Hozzáférés megtagadva (Engedélyezés) Microsoft Graph API kategóriát választva további segítséget és támogatást kap erről a témakörről. 

**A Microsoft Graph-t szeretném használni, de nem tudom, hol kezdjem**

A Microsoft-fiókkal kapcsolatos Graph olvassa el az alábbi cikkeket:

- [A Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Az identitás- és hozzáférés-kezelés áttekintése a Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph-alkalmazások Graph első lépések](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – A Microsoft Graph API-k tesztelése a bérlői fiókban vagy a bemutató bérlői fiókban

**Szeretném használni a Microsoft Graph, de támogatja az 1.0-s címtár API-kat, amelyekre szükségem van?**

A Microsoft Graph a címtár-, identitás- és hozzáférés-kezeléshez ajánlott API. Az Azure AD-szolgáltatásokban és a Microsoft-szolgáltatásokban lehetséges Graph azonban továbbra Graph. Tekintse át az alábbi cikkeket, amelyek kiemelik a legújabb különbségeket, hogy segítsék a választását:

- [Erőforrástípus-különbségek az Azure AD-Graph És a Microsoft-Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Az Azure AD-szolgáltatások és a Microsoft-Graph közötti Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Az Azure AD és a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Amikor lekérdezem *a felhasználói* objektumot, annak számos tulajdonsága hiányzik**

`GET https://graph.microsoft.com/v1.0/users`csak 11 tulajdonságot ad vissza, mivel a Microsoft  Graph automatikusan kiválaszt egy alapértelmezett felhasználói tulajdonságkészletet. Ha más felhasználói tulajdonságokra is *szüksége* van, $select az alkalmazás számára szükséges tulajdonságokat. Először próbálja ki a **Microsoft Graph Explorerben.**

**A felhasználói tulajdonság egyes értékei *null értékűek* annak ellenére, hogy tudom, hogy be vannak állítva**

A legvalószínűbb magyarázat az, hogy az alkalmazás *User.ReadBasic.All* engedélyt kapott. Ez lehetővé teszi, hogy az alkalmazás csak korlátozott számú felhasználói tulajdonságot olvasson be, és minden más tulajdonságot null értékként ad vissza, még akkor is, ha korábban be vannak állítva. Adjon helyette *User.Read.All engedélyt* az alkalmazásnak.

További információ: [A Microsoft Graph jogosultságai.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Problémáim vannak az OData-lekérdezési paraméterek használatával a kérések adatainak szűréséhez**

Bár a Microsoft Graph az OData-lekérdezés paramétereinek széles választékát támogatja, a Microsoft-címtárszolgáltatások (a *címtárobjektumtól* öröklött erőforrások) sok paramétert nem Graph. A Microsoft Graph szolgáltatásban állandók az Azure AD-ban Graph korlátozások:

1. **Nem támogatott:**$count, $search és $filter *null értékekkel vagy* *nem null értékekkel*
2. **Nem támogatott:**$filter tulajdonságokat támogat (lásd az erőforrásokkal kapcsolatos témaköröket, amelyekről a tulajdonságok szűrhetők)
3. **Nem támogatott:** egyszerre lapozás, szűrés és rendezés
4. **Nem támogatott:** kapcsolat szűrése. Megkeresheti például az Egyesült Királyságban található mérnöki csoport összes tagját.
5. **Részleges támogatás:**$orderby *(displayName* és userPrincipalName csak) és *csoport*
6. Részleges **támogatás:** az $filter (csak *eq* *,* kezdődik *,* vagy *,* és korlátozott *bármely*) támogatása, az $expand (egyetlen objektum kapcsolatának kibontása az összes kapcsolatot visszaadja, de az objektumok kapcsolatainak gyűjteménye korlátozott)

További információ: [Válaszok testreszabása lekérdezési paraméterekkel.](https://docs.microsoft.com/graph/query-parameters)

**A híváshoz hívott API nem működik – hol tudok további teszteket tesztelni?**

**Microsoft Graph Explorer** – Tesztelje a Microsoft Graph API-ját a bérlői  fiókjában vagy egy demo bérlőben, és tekintse meg a minta lekérdezéseket a Microsoft Graph Explorerben.

**Adatok lekérdezésekor úgy tűnik, hiányos adatok halmazát kapom vissza**

Ha egy gyűjteményt (például felhasználókat) szeretne lekérdezni, a Microsoft Graph kiszolgálóoldali lapkorlátokat használ, így a találatok mindig egy alapértelmezett oldalmérettel nyomtatódnak vissza. Az alkalmazásnak mindig lapokkal kell átlaposodni a szolgáltatásból visszaadott gyűjteményeket.

További információ:

- [Ajánlott Graph Microsoft-alkalmazások](https://docs.microsoft.com/graph/best-practices-concept)
- [A Microsoft Graph adatok lapozása az alkalmazásban](https://docs.microsoft.com/graph/paging)

**Az app túl lassú, és le van szabályozás alatt. Milyen fejlesztéseket lehet javítására?**

A helyzettől függően számos különböző lehetőség áll a rendelkezésére az alkalmazás végrehajtásához, és bizonyos esetekben kevésbé valószínű, hogy a szolgáltatás le kellene mondania (ha túl sok hívást kezdeményez).

További információt az alábbi témakörökben találhat:

- [Ajánlott Graph Microsoft-alkalmazások](https://docs.microsoft.com/graph/best-practices-concept)
- [Kötegkérések](https://docs.microsoft.com/graph/json-batching)
- [Változások követése a különbözeti lekérdezésen keresztül](https://docs.microsoft.com/graph/delta-query-overview)
- [Értesítés a változásokról webhooksen keresztül](https://docs.microsoft.com/graph/webhooks)
- [Szabályozási útmutató](https://docs.microsoft.com/graph/throttling)

**Hol találok további információt a hibákról és az ismert problémákról?**

- [A Microsoft Graph válaszokkal kapcsolatos információk](https://docs.microsoft.com/graph/errors)
- [A Microsoft-fiók ismert Graph](https://docs.microsoft.com/graph/known-issues)

**Hol tudom ellenőrizni a szolgáltatások elérhetőségét és csatlakozását?**

A Microsoft Graph szolgáltatáson keresztül elérhető szolgáltatások elérhetősége és csatlakozása hatással lehet a Microsoft Graph.

- Ha Azure Active Directory szolgáltatás állapotát, ellenőrizze az Azure állapotlapján felsorolt **Biztonsági és** identitásszolgáltatások [állapotát.](https://azure.microsoft.com/status/)
- A Microsoft Office szolgáltatáshoz hozzájáruló szolgáltatások Graph a Szolgáltatás állapota irányítópulton felsorolt szolgáltatások [állapotát Office ellenőrizheti.](https://portal.office.com/adminportal/home#/servicehealth)
