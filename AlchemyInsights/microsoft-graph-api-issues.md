---
title: A Microsoft Graph API-val kapcsolatos problémák
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
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714150"
---
# <a name="microsoft-graph-api-issues"></a>A Microsoft Graph API-val kapcsolatos problémák

Ez a témakör az Azure AD Graph API-t még használó fejlesztőkre is vonatkozhat. Erősen javasoljuk  azonban, hogy a Microsoft Graphot minden címtár-, identitás- és hozzáférés-kezelési esethez használja.

**Hitelesítési vagy engedélyezési problémák**

- Ha az  app nem tud jogkivonatokat szerezni a Microsoft Graph hívásához, válassza a Microsoft Graph-kategória Hozzáférési jogkivonat **(Authentication)** kategóriájának lehívásával kapcsolatos problémát, és további súgót és támogatást kap erről a témakörről.
- Ha az app **401-es vagy 403-as** engedélyezési hibát kap a Microsoft Graph hívása közben, válassza a Hozzáférés megtagadva **(Engedélyezés)** Microsoft Graph API-kategóriát, ha további konkrét segítséget és támogatást kap erről a témakörről.

**A Microsoft Graphot szeretném használni, de nem tudom, hol kezdjem**

- [A Microsoft Graph áttekintése](https://docs.microsoft.com/graph/overview)
- [Az identitás- és hozzáférés-kezelés áttekintése a Microsoft Graphban](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph-alkalmazások építésének első lépések](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – A Microsoft Graph API-k tesztelése a bérlői vagy a demo bérlői fiókban

**Szeretném használni a Microsoft Graphot, de támogatja a szükséges v1.0-s címtár API-kat?**

A Microsoft Graph a címtár- és identitáskezeléshez, valamint a hozzáférés-kezeléshez ajánlott API. Az Azure AD Graph és a Microsoft Graph szolgáltatásai között azonban továbbra is van néhány hiányosságok. Tekintse át az alábbi cikkeket, amelyek kiemelik a legfrissebb különbségeket, hogy segítsék a választást:

- [Erőforrástípusbeli különbségek az Azure AD Graph és a Microsoft Graph között](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Az Azure AD Graph és a Microsoft Graph közötti tulajdonságkülönbségek](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Módszerbeli különbségek az Azure AD és a Microsoft Graph között](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**A híváshoz hívott API nem működik – hol lehet további tesztelést?**

**Microsoft Graph Explorer** – Tesztelje a Microsoft Graph API-kat  a bérlői vagy a bemutató-bérlői fiókjában, és tekintse meg a Minta lekérdezéseket a Microsoft Graph Explorerben.

**Az app túl lassú, és le van szabályozás alatt. Milyen fejlesztéseket tudok tenni?**

A forgatókönyvtől függően számos lehetőség áll rendelkezésére az alkalmazás teljesítményének végrehajtásához, és bizonyos esetekben kevésbé van kivetve a szolgáltatás által lekordolt szabályozás (ha túl sok hívást kezdeményez).

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
- A Microsoft Graph-hoz hozzájáruló Office-szolgáltatások esetén ellenőrizze az Office szolgáltatásállapot-irányítópultján felsorolt [szolgáltatások állapotát.](https://portal.office.com/adminportal/home#/servicehealth)

A Microsoft Graph engedélyezési hibáinak számos különböző oka lehet, amelyek nagy része 401-es vagy 403-as hibát generál. Az alábbiak például engedélyezési hibákhoz vezethetnek:

- Helytelen [hozzáférési jogkivonat beszerzési folyamatok](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Rosszul konfigurált [engedély hatókörök](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [Jóváhagyás](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) hiánya

**_Az Azure Active Directory-hitelesítési tár (ADAL) és az Azure AD Graph API (AAD Graph) támogatásának vége_* _

_*2020. június 30-től**, az ADAL és az Azure AD Graph szolgáltatásban nem adjuk hozzá az új funkciókat. A jövőben is biztosítani fogunk technikai támogatási és biztonsági frissítéseket, funkciófrissítéseket azonban nem.

**2022. június 30-án** véget ér az ADAL és az Azure AD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást vagy biztonsági frissítéseket.

Az ADAL-t a meglévő operációs rendszerverziókban használó appok ez idő után is működni fognak, de nem fognak technikai támogatást vagy biztonsági *frissítéseket kapni.*

Az Azure AD Graph-et ezt követően használó appok a továbbiakban nem kaphatnak választ az Azure AD Graph végponttól.

**ADAL-áttelepítés**

Javasoljuk, hogy frissítsen a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) szolgáltatásra, amely a legújabb funkciókat és biztonsági frissítéseket használja.

Ha Microsoft-appokat használ, tudja, hogy a Microsoft a támogatási határidő lejárta előtt átemeli az alkalmazásait a MSAL szolgáltatásba, és biztosítja, hogy a MSAL folyamatos biztonsági és funkciófejlesztések hasznára legyen.

1. [Az ADAL GYIK elolvasása](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [További információ az appok áttelepítéséről platformonként](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ha segítségre van szüksége annak megértéséhez, hogy melyik appja használja az ADAL-t, javasoljuk, hogy tekintse át az appok összes forráskódját, és ha lehetséges, bármely internetszolgáltatóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft terméktámogatási szolgálata a bérlői fiókban a nem Microsoft rendszerű ADAL-appok listáját is biztosítja.

**AAD Graph-áttelepítés**

Az Azure AD Graph-et használó alkalmazások esetében kövesse az útmutatót az Azure AD Graph-appok Microsoft Graphba való [áttelepítéséhez.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Az áttelepítési ellenőrzőlista segít az első lépésekben](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Az Azure-appok regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot. Javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, forduljon bármely szoftverszolgáltatóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft ügyfélszolgálata az AAD Graph-használat teljes listáját is biztosítja a bérlői fiókjában.
3. Ahhoz, hogy az app hozzáférjen a Microsoft Graph adataihoz, a felhasználónak vagy a rendszergazdának a jóváhagyási folyamaton keresztül meg kell adnia neki a megfelelő engedélyeket. A [Microsoft Graph engedélyeinek hivatkozása](https://docs.microsoft.com/graph/permissions-reference) felsorolja a Microsoft Graph API-k egyes fő készletével társított engedélyeket. Útmutatást is nyújt az engedélyek használatára vonatkozóan.
