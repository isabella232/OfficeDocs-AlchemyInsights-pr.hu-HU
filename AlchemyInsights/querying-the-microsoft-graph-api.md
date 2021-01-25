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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974420"
---
# <a name="querying-the-microsoft-graph-api"></a>A Microsoft Graph API lekérdezése

Ez a témakör az Azure AD Graph API-t még használó fejlesztőkre is vonatkozhat. Erősen javasoljuk **azonban,** hogy a Microsoft Graphot minden címtár-, identitás- és hozzáférés-kezelési esethez használja.

**Hitelesítési vagy engedélyezési problémák**

- Ha az  app nem tud jogkivonatokat szerezni a Microsoft Graph hívásához, válassza a Microsoft Graph-kategória Hozzáférési jogkivonat **(Hitelesítés)** esetén a probléma megoldását, ha további segítségre és támogatásra van szüksége a témakörben.
- Ha az app **401-es vagy 403-as** engedélyezési hibát kap a Microsoft Graph hívása közben, válassza a Hozzáférés megtagadva **(Engedélyezés)** Microsoft Graph API-kategóriát, ha további konkrét segítséget és támogatást kap erről a témakörről.

**A Microsoft Graphot szeretném használni, de nem tudom, hol kezdjem**

A Microsoft Graphról az alábbi cikkből olvashat bővebben:

- [A Microsoft Graph áttekintése](https://docs.microsoft.com/graph/overview)
- [Az identitás- és hozzáférés-kezelés áttekintése a Microsoft Graphban](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph-alkalmazások építésének első lépések](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – A Microsoft Graph API-k tesztelése a bérlői vagy a bemutató bérlői webhelyen

**Szeretném használni a Microsoft Graphot, de támogatja a szükséges v1.0-s címtár API-kat?**

A Microsoft Graph a címtár- és identitáskezeléshez, valamint a hozzáférés-kezeléshez ajánlott API. Az Azure AD Graph és a Microsoft Graph szolgáltatásai között azonban továbbra is van néhány hiányosságok. Tekintse át az alábbi cikkeket, amelyek kiemelik a legfrissebb különbségeket, hogy segítsék a választást:

- [Erőforrástípusbeli különbségek az Azure AD Graph és a Microsoft Graph között](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Az Azure AD Graph és a Microsoft Graph közötti tulajdonságkülönbségek](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Módszerbeli különbségek az Azure AD és a Microsoft Graph között](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Amikor lekérdezem *a felhasználói* objektumot, számos tulajdonsága hiányzik**

`GET https://graph.microsoft.com/v1.0/users`csak 11 tulajdonságot ad vissza, mivel a  Microsoft Graph automatikusan kiválasztja a visszaadni kívánt alapértelmezett felhasználói tulajdonságokat. Ha más felhasználói *tulajdonságokra* van szüksége, $select az alkalmazás igényeinek megfelelő tulajdonságokat. Először próbálja ki a **Microsoft Graph Explorerben.**

**Egyes felhasználói tulajdonságértékek *null értékűek* annak ellenére, hogy tudom, hogy be vannak állítva**

A legvalószínűbb magyarázat az, hogy az alkalmazás a *User.ReadBasic.All* engedélyt is megadta. Ez lehetővé teszi, hogy az alkalmazás beolvassa a felhasználói tulajdonságok egy bizonyos készletét, és az összes többi tulajdonságot null értékként adja vissza, még akkor is, ha korábban be vannak állítva. Próbálja meg ehelyett *a User.Read.All* engedélyt kiadó alkalmazást.

További információt a [Microsoft Graph felhasználói engedélyeiben található.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Problémáim vannak az OData-lekérdezési paraméterek használatával a kérések adatainak szűréséhez**

Bár a Microsoft Graph az OData-lekérdezési paraméterek széles körét támogatja, a Microsoft Graph címtárszolgáltatásai (a *címtárobjektumtól öröklött* erőforrások) nem támogatják teljes mértékben ezeket a paramétereket. Az Azure AD Graph-ban ugyanazok a korlátozások maradnak meg, amelyek a Legtöbb esetben a Microsoft Graphban is fennállnak:

1. **Nem támogatott:**$count, $search és $filter *null* vagy nem *null érték esetén*
2. **Nem támogatott:**$filter tulajdonságokon (lásd az erőforrásokkal kapcsolatos témaköröket, amelyeken szűrhető tulajdonságok vannak)
3. **Nem támogatott:** egyszerre lapozás, szűrés és rendezés
4. **Nem támogatott:** kapcsolat szűrése. Megkeresheti például az Egyesült Királyságban található mérnöki csoport összes tagját.
5. **Részleges támogatás:**$orderby *felhasználón* (displayName és userPrincipalName csak) és *csoporton*
6. Részleges **támogatás:**$filter (csak *eq*, *kezdetek,* *vagy*, és *,* és *korlátozott)* támogatás, az $expand (egyetlen objektum kapcsolatának kibontása visszaadja az összes kapcsolatot, de az objektumok kapcsolatainak kibontása korlátozott)

További információt a válaszok [testreszabása lekérdezési paraméterekkel.](https://docs.microsoft.com/graph/query-parameters)

**A híváshoz hívott API nem működik – hol lehet további teszteket tesztelni?**

**Microsoft Graph Explorer** – Tesztelje a Microsoft Graph API-kat  a bérlői vagy a demo bérlői fiókjában, és tekintse meg a Minta lekérdezéseket a Microsoft Graph Explorerben.

**Adatok lekérdezésekor úgy tűnik, hiányos adatok halmazát kapom vissza**

Ha egy gyűjteményt (például a felhasználókat) lekérdezést *használ,* a Microsoft Graph kiszolgálóoldali lapkorlátokat használ, így az eredmények mindig alapértelmezett oldalmérettel nyomtatódnak vissza. Az alkalmazásnak mindig a szolgáltatásból visszaadott gyűjtemények lapjára kell számítania.

További információ:

- [Ajánlott eljárások a Microsoft Graphhoz](https://docs.microsoft.com/graph/best-practices-concept)
- [Microsoft Graph-adatok lapozása az alkalmazásban](https://docs.microsoft.com/graph/paging)

**Az app túl lassú, és le van szabályozás alatt. Milyen fejlesztéseket tudok tenni?**

A helyzettől függően számos különböző lehetőség áll a rendelkezésére az alkalmazás végrehajtásához, és bizonyos esetekben kevésbé van kivetve a szolgáltatás szabályozásának (ha túl sok hívást kezdeményez).

További információt az alábbi témakörökben találhat:

- [Ajánlott eljárások a Microsoft Graphhoz](https://docs.microsoft.com/graph/best-practices-concept)
- [Kötegkérések](https://docs.microsoft.com/graph/json-batching)
- [Változások követése a különbözeti lekérdezésen keresztül](https://docs.microsoft.com/graph/delta-query-overview)
- [Értesítés a változásokról webhookokon keresztül](https://docs.microsoft.com/graph/webhooks)
- [Szabályozási útmutató](https://docs.microsoft.com/graph/throttling)

**Hol találok további információt a hibákról és az ismert problémákról?**

- [A Microsoft Graph hibare adott válaszokkal kapcsolatos adatai](https://docs.microsoft.com/graph/errors)
- [A Microsoft Graph ismert problémái](https://docs.microsoft.com/graph/known-issues)

**Hol tudom ellenőrizni a szolgáltatás elérhetőségét és csatlakozását?**

A Microsoft Graphon keresztül elérhető mögöttes szolgáltatások elérhetősége és csatlakozása hatással lehet a Microsoft Graph általános elérhetőségére és teljesítményére.

- Az Azure Active Directory szolgáltatásállapota esetén ellenőrizze az Azure állapotlapján felsorolt **Biztonsági és** identitásszolgáltatások [állapotát.](https://azure.microsoft.com/status/)
- A Microsoft Graph-hoz hozzájáruló Office-szolgáltatások állapotát az Office szolgáltatásállapot-irányítópultján [ellenőrizheti.](https://portal.office.com/adminportal/home#/servicehealth)
