---
title: A Microsoft Graph API-jának problémái
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
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975895"
---
# <a name="microsoft-graph-api-issues"></a>A Microsoft Graph API-jának problémái

Ez a témakör azokra a fejlesztőkre is vonatkozhat, akik továbbra is az Azure AD Graph API-t használják. Azonban erősen  ajánlott a Microsoft Graph használata az összes címtár-, identitás- és hozzáférés-kezelési esethez.

**Hitelesítési vagy engedélyezési problémák**

- Ha az  app nem tud jogkivonatokat szerezni a Microsoft Graph hívásához, válassza a Probléma a hozzáférési jogkivonat **(hitelesítés)** Microsoft Graph kategóriával, és további segítséget és támogatást kap erről a témakörről.
- Ha appja **401-es vagy 403-as** engedélyezési hibát kap a Microsoft Graph hívása közben, a Hozzáférés megtagadva (Engedélyezés) Microsoft Graph API kategóriát választva további segítséget és támogatást kap erről a témakörről. 

**A Microsoft Graph-t szeretném használni, de nem tudom, hol kezdjem**

- [A Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Az identitás- és hozzáférés-kezelés áttekintése a Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph-alkalmazások Graph első lépések](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – A Microsoft Graph API-k tesztelése a bérlői fiókban vagy a bemutató bérlői fiókban

**Szeretném használni a Microsoft Graph, de támogatja az 1.0-s címtár API-kat, amelyekre szükségem van?**

A Microsoft Graph a címtár-, identitás- és hozzáférés-kezeléshez ajánlott API. Az Azure AD-szolgáltatásokban és a Microsoft-szolgáltatásokban lehetséges Graph azonban továbbra Graph. Tekintse át az alábbi cikkeket, amelyek kiemelik a legújabb különbségeket, hogy segítsék a választását:

- [Erőforrástípus-különbségek az Azure AD-Graph És a Microsoft-Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Az Azure AD-szolgáltatások és a Microsoft-Graph közötti Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Az Azure AD és a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**A híváshoz hívott API nem működik – hol tudok további teszteket tesztelni?**

**Microsoft Graph Explorer** – Tesztelje a Microsoft Graph API-ját a bérlői  fiókjában vagy egy demo bérlőben, és tekintse meg a minta lekérdezéseket a Microsoft Graph Explorerben.

**Az app túl lassú, és le van szabályozás alatt. Milyen fejlesztéseket lehet javítására?**

A helyzettől függően számos lehetőség áll a rendelkezésére az alkalmazás végrehajtásához, és bizonyos esetekben kevésbé valószínű, hogy a szolgáltatás le kellene mondania (ha túl sok hívást kezdeményez).

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

A Microsoft Graph engedélyezési hibáinak számos különböző oka lehet, amelyek nagy része 401-es vagy 403-as hibát generál. Az alábbi hibák például engedélyezési hibákhoz vezethetnek:

- Helytelen [hozzáférési jogkivonat beszerzési folyamatok](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Rosszul konfigurált [engedély hatókörök](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [Jóváhagyás](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) hiánya

***Az Azure Active Directory Authentication Library (ADAL) és az Azure AD Graph API (AAD-hitelesítés) támogatása Graph)***

**2020. június 30-án** kezdődően nem adjuk hozzá az új funkciókat az ADAL-hoz és az Azure AD-Graph. A jövőben is biztosítani fogunk technikai támogatási és biztonsági frissítéseket, funkciófrissítéseket azonban nem.

**2022.** június 30-ával kezdődően véget ér az ADAL és az Azure AD Graph támogatása, és a továbbiakban nem nyújtunk technikai támogatást és biztonsági frissítéseket.

Az ADAL-t használó appok a meglévő operációs rendszerverziókban továbbra is működnek, de semmilyen technikai támogatást vagy biztonsági frissítést nem *fognak kapni.*

Az Azure AD-t használó Graph ezt követően előfordulhat, hogy a továbbiakban nem kap válaszokat az Azure AD Graph végponttól.

**ADAL-áttelepítés**

Javasoljuk, hogy frissítsen a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) szolgáltatásra, amely a legújabb funkciókat és biztonsági frissítéseket használja.

Ha Microsoft-appokat használ, tudja, hogy a Microsoft a támogatási határidő lejárta előtt át fogja átemelni az alkalmazásait az MSAL-be, hogy azok kihasználják a MSAL folyamatos biztonsági és funkciófejlesztésének előnyét.

1. [Az ADAL GYIK elolvasása](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [További információ az appok áttelepítéséről platformonként](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ha segítségre van szüksége annak megértéséhez, hogy melyik appja használja az ADAL-t, javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, bármilyen internetszolgáltatóhoz vagy alkalmazásszolgáltatóhoz is érdemes segítséget kérnie. A Microsoft terméktámogatási szolgálata a bérlői fiókban a nem Microsoft rendszerű ADAL-appok listáját is biztosítja.

**AAD Graph-áttelepítés**

Az Azure AD Graph-t használó alkalmazások esetén kövesse az Azure AD Graph-appok microsoftos [Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Az áttelepítési ellenőrzőlista segít az első lépésekben](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Az Azure-appok regisztrációs portálján látható, hogy mely alkalmazások használják az AAD Graphot. Javasoljuk, hogy tekintse át az összes app forráskódját, és ha lehetséges, forduljon bármely szoftverszolgáltatóhoz vagy alkalmazásszolgáltatóhoz. A Microsoft ügyfélszolgálata a bérlői fiókjában az AAD-használat Graph listáját is meg tudja Önnek adni.
3. Ahhoz, hogy az app hozzáférjen az adatokhoz a Microsoft Graph-ban, a felhasználónak vagy a rendszergazdának egy jóváhagyási folyamaton keresztül meg kell adnia neki a megfelelő engedélyeket. A [Microsoft Graph az](https://docs.microsoft.com/graph/permissions-reference) engedélyekre vonatkozó hivatkozás felsorolja az egyes microsoftos Graph API-khoz társított engedélyeket. Útmutatást is nyújt az engedélyek használatára vonatkozóan.
